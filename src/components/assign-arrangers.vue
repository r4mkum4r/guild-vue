<template>
  <div id="arrange-and-approve-container" class="row">
    <div class="col col-8 nested-grid">
      <div class="box">
        <div class="box-padded">
          <div id="arrange-and-approve-content" class="profile-section profile-field-section">
            <div class="row">
              <div class="col col-3 hide-small-screen">
                <div class="profile-label right">
                  <h5 class="sub-header">Arrangers</h5>
                  <button
                    type="button"
                    id="assign-arrangers"
                    class="modal-opener btn btn-text-action btn-small btn-no-margin"
                    data-target-modal="arrangers"
                  >
                    <span class="btn-label no-side-padding" @click="onManage">Manage</span>
                  </button>
                </div>
              </div>
              <div class="col col-4">
                <div id="arrangers" class="col-10 middled">No Arranger selected</div>
              </div>
              <div v-for="arranger in arrangers" :key="arranger">
                <div class="input-group">
                  {{arranger}}
                  <input
                    type="checkbox"
                    id="6486691"
                    class="user-selection"
                    value="6486691"
                    @change="onSelectionChange"
                  >
                  <label for="6486691">Adam TestFour</label>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component({})
export default class AssignArrangers extends Vue {
  arrangers = [1, 2, 3];
  selectedUsers = [];
  onManage() {}

  onSelectionChange(evt: Object) {
    console.log(evt);
  }
}
</script>

