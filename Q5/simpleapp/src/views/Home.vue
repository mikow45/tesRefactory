<style scoped src="@/assets/home.css"></style>
<template>
  <div class="home">
    <div class="container mt-home">
      <div class="greetingbox col-lg-4">
        <div class="greeting">
          <div class="ilustrasi-box">
            <img class="ilustrasi" src="@/assets/home_img/bookandpen.svg" alt="">
          </div>
          <div class="greeting-text">
              <h5>Hallo, Sam!</h5>
              <p>You have 2 tasks left for today, Already completed Task today?</p>
          </div>
        </div>
      </div>
      <div class="mt-task col-lg-8">
        <h1>Task For Today</h1>
        <div class="task-header">
          <!-- Button trigger modal -->
          <button type="button" class="btn createbtn" data-bs-toggle="modal" data-bs-target="#exampleModal">
             <img src="@/assets/home_img/plus.svg" alt="">
            Create New
          </button>
        <div class="input-group mb-3">
          <input type="text" class="form-control" placeholder="Cari" aria-label="Cari" aria-describedby="basic-addon2">
          <div class="input-group-append">
            <button class="btn btn-outline-secondary" type="button"><i class="fa fa-search"></i></button>
          </div>
        </div>
        </div>
        <!-- task list -->
        <project></project>
      </div>
    </div>
          <!-- Modal -->
          <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
            <div class="modal-dialog">
              <div class="modal-content">
                <div class="modal-header">
                  <h5 class="modal-title" id="exampleModalLabel">New Task</h5>
                  <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                  <div class="input-model">
                  <label class="form-label model-title">Title</label>
                  <input type="text" class="form-control" placeholder="Daily Standup Project">
                </div>
                <div class="input-model">
                  <label class="form-label mt-3">Description</label>
                  <textarea class="form-control area" placeholder="lorem ipsum"></textarea>
                </div>
                </div>
                <div class="modal-footer">
                  <button type="button" class="btn cancel" data-bs-dismiss="modal">Cancel</button>
                  <button type="button" class="btn yes">Create Task</button>
                </div>
              </div>
            </div>
          </div>
  </div>
</template>
<script src="./js/home.js"></script>
<script>
// @ is an alias to /src
import project from "@/components/tasklist.vue"
// import { component } from "vue/types/umd"
export default {
  name: "Home",
  components:{
    project,
  }
};
</script>
