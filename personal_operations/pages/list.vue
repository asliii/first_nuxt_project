<template>
<div class="container">
<h4>My Staff List (This page using bootsrap4! Please look at nuxt.config.js)</h4>
<table class="table">
<thead>
<th>#</th>
<th>Name</th>
<th>Task</th>
</thead>
<tbody>
<tr v-for="(staff, index) in staff_list">
<td>{{ index }}</td>
<td>{{ staff.name }}</td>
<td>{{ staff.task }}</td>
</tr>
</tbody>
</table>
</div>
</template>

<script>
export default {
     asyncData (context) {

    return { staff_list: [{'name': 'Aslıhan Nurcan Çetin', 'task': 'Boss and Computer Engineer'}] }
  },
  fetch () {
    // The `fetch` method is used to fill the store before rendering the page
  },
  head () {
    // Set Meta Tags for this Page
  },
}

</script>