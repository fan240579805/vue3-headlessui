<template>
  <SwitchGroup>
    <div class="flex items-center">
      <SwitchLabel class="mr-4">点我</SwitchLabel>
      <Switch
        v-model="enabled"
        :class="enabled ? 'bg-blue-600' : 'bg-gray-200'"
        class="relative inline-flex items-center h-6 transition-colors rounded-full w-11 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
      > 
        <span
          :class="enabled ? 'translate-x-6' : 'translate-x-1'"
          class="span_wrap inline-block w-4 h-4 transition-transform transform bg-white rounded-full span_wrap"
        />
      </Switch>
    </div>
  </SwitchGroup>
</template>

<script>
import { ref } from "vue";
import { Switch, SwitchGroup, SwitchLabel } from "@headlessui/vue";

export default {
  components: { Switch, SwitchGroup, SwitchLabel },

  setup() {
    const enabled = ref(false);

    return { enabled };
  },
};
</script>

<style>
  .span_wrap{
    background-color: red;
  }    
</style>
