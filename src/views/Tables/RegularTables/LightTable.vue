<template>
  <b-card no-body>
    <b-card-header class="border-0">
      <h3 class="mb-0">Activity Table</h3>
      <form>
        <div
          class="form-group m-0 p-0 col-sm-12 d-flex flex-column justify-content-center align-items-end"
        >
          <label for="exampleFormControlSelect1"
            >Select session to filter activity results</label
          >
          <select class="form-control col-sm-3" id="exampleFormControlSelect1">
            <option>2017/2018</option>
            <option>1</option>
            <option>2</option>
            <option>3</option>
            <option>4</option>
          </select>
        </div>
      </form>
    </b-card-header>

    <el-table
      class="table-responsive table"
      header-row-class-name="thead-light"
      :data="projects"
    >
      <el-table-column label="Hostel" min-width="310px" prop="name">
        <template v-slot="{ row }">
          <b-media no-body class="align-items-center">
            <b-media-body>
              <span class="font-weight-600 name mb-0 text-sm">{{
                row.title
              }}</span>
            </b-media-body>
          </b-media>
        </template>
      </el-table-column>
      <el-table-column label="Room" prop="budget" min-width="140px">
      </el-table-column>

      <el-table-column label="Status" min-width="170px" prop="status">
        <template v-slot="{ row }">
          <badge class="badge-dot mr-4" type="">
            <i :class="`bg-${row.statusType}`"></i>
            <span class="status" :class="`text-${row.statusType}`">{{
              row.status
            }}</span>
          </badge>
        </template>
      </el-table-column>

      <el-table-column label="Time left" prop="completion" min-width="240px">
        <template v-slot="{ row }">
          <div class="d-flex align-items-center">
            <span class="completion mr-2">{{ row.completion }}%</span>
            <div>
              <base-progress :type="row.statusType" :value="row.completion" />
            </div>
          </div>
        </template>
      </el-table-column>

      <el-table-column label="Action" prop="completion" min-width="200px">
        <template>
          <div class="d-flex align-items-center">
            <button
              class="btn btn-outline-dark py-1 px-sm-2"
              @click="printHostelData"
            >
              Print receipt
            </button>
          </div>
        </template>
      </el-table-column>
    </el-table>

    <!-- <b-card-footer class="py-4 d-flex justify-content-end">
            <base-pagination v-model="currentPage" :per-page="10" :total="50"></base-pagination>
        </b-card-footer> -->
  </b-card>
</template>
<script>
import projects from "./../projects";
import { Table, TableColumn } from "element-ui";
export default {
  name: "light-table",
  components: {
    [Table.name]: Table,
    [TableColumn.name]: TableColumn,
  },
  data() {
    return {
      projects,
      currentPage: 1,
    };
  },
  methods:{
     printHostelData: function() {
      window.print();
    }
  },
};
</script>
