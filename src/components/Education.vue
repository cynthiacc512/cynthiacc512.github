<template>
    <section class="container" id="education">
      <h1>Education</h1>
      <div
          v-for="(education, index) in educations"
          :key="index"
          class="edu-info"
      >
        <h4>{{education.title}}</h4>
        <h5>{{education.description}}</h5>
        <h5>{{education.date}}</h5>
      </div>
    </section>
</template>

<script>
export default {
    name: 'Education',
    data: () => {
      return ({
        educations: [
          {
            title: 'Institut Teknologi Harapan Bangsa',
            description: 'Informatics',
            date: '2018-2022',
          },
          {
            title: 'Bangkit Academy led by Google, Tokopedia, Gojek, & Traveloka',
            description: 'Cloud Computing Student',
            date: 'Feb 2021-Jul 2021',
          },
        ],
      })
    },
}
</script>