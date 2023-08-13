<template>
  <div class="container">
    <div class="employee">
      <table>
        <tr>
          <th class="user">
            <input type="checkbox" />
            <span>Employees</span>
          </th>
        </tr>

        <div v-for="data in datas" :key="data.id">
          <tr>
            <td class="profile">
              <input type="checkbox" />
              <img src="../user/1.jpeg" alt="profile" />
              <span>{{ data.name }}</span>
            </td>
          </tr>
        </div>
      </table>
    </div>
    <div class="data">
      <table>
        <div class="headerData">
          <tr class="one">
            <th class="header">Location</th>
            <th class="header">Email</th>
            <th class="header">Phone</th>
            <th class="header">Department</th>
            <th class="header">Employee Code</th>
            <th class="header">Custom tag</th>
            <th class="header">Positions</th>
            <th class="header">NRC</th>
            <th class="header">Manager</th>
            <th class="header">Manager Position</th>
            <th class="header">Joined Date</th>
            <th class="header">Terminate Date</th>
          </tr>

          <tr v-for="data in datas" :key="data.id" class="data">
            <td class="tableData">{{ data.location }}</td>
            <td class="tableData">{{ data.email }}</td>
            <td class="tableData">{{ data.phone }}</td>
            <td class="tableData">{{ data.department }}</td>
            <td class="tableData">{{ data.employeeCode }}</td>
            <td class="tableData">{{ data.tag }}</td>
            <td class="tableData">{{ data.positions }}</td>
            <td class="tableData">{{ data.nrc }}</td>
            <td class="tableData">{{ data.manager }}</td>
            <td class="tableData">{{ data.managerPosition }}</td>
            <td class="tableData">{{ data.date }}</td>
            <td class="tableData">{{ data.terminate }}</td>
          </tr>
        </div>
      </table>
    </div>
  </div>
</template>

<script setup>
import { useData } from "../store/EmployeeData";
import { storeToRefs } from "pinia";

const employeeData = useData();
const { datas } = storeToRefs(employeeData);
</script>

<style scoped>
.container {
  display: flex;
}
.employee {
  position: sticky;
  left: 0;
  background-color: var(--light);
}
.profile {
  display: flex;
  margin: 7px 20px;
  align-items: center;
}
.user {
  margin: 20px;
  display: flex;
  align-items: center;
  width: 250px;
  height: 30px;
}
span {
  margin-left: 10px;
}
th {
  font-weight: 500;
  text-align: left;
}
input {
  margin-right: 20px;
}
img {
  width: 20px;
  border-radius: 50%;
  margin: 10.5px;
}
.bar {
  width: 100%;
  height: 0.05rem;
  background-color: rgb(220, 208, 208);
}
.headerData {
  width: calc(100vw - 30vw);
  overflow: auto;
}
.header {
  padding: 25px;
  margin-bottom: 5px;
}
.tableData {
  min-width: 250px;
  margin: 20px;
  align-items: center;
  padding: 19px;
}
.one {
  margin-bottom: 5px;
}
</style>
