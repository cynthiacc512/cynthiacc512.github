<template>
    <section class="container" id="work-experience">
      <h1>Work Experience</h1>
      <table class="table table-dark table-striped">
        <thead>
          <tr>
            <th>Company</th>
            <th>Role</th>
            <th>Status</th>
            <th>Period</th>
          </tr>
        </thead>
        <tbody>
          <tr
            v-for="(experience, index) in experiences"
            :key="index"
          >
            <td>{{experience.company}}</td>
            <td>{{experience.role}}</td>
            <td>{{experience.status}}</td>
            <td>{{experience.period}}</td>
          </tr>
        </tbody>
      </table>
    </section>
</template>

<script>
export default {
    name: 'WorkExperience',
    data: () => {
      return ({
        experiences: [
          {
            company: 'Frontstep',
            role: 'Front End Developer',
            status: 'Internship',
            period: 'Jun 2021 - Jul 2021',
          },
          {
            company: 'Frontstep',
            role: 'UI/UX Designer',
            status: 'Partime',
            period: 'May 2021 - Jul 2021',
          },
          {
            company: 'Magika Studio',
            role: 'Junior Content Designer',
            status: 'Partime',
            period: 'Agu 2020 - Apr 2021',
          },
          {
            company: 'Dollan',
            role: 'Designer Grafis dan UI/UX Designer',
            status: 'Freelance',
            period: 'Agu 2020 - Sep 2020',
          },
          {
            company: 'Self Employed',
            role: 'Freelance UI/UX Designer',
            status: 'Freelance',
            period: 'Jun 2019 - Jun 2020',
          },
          {
            company: 'Self Employed',
            role: 'Freelance Front End Web Developer',
            status: 'Freelance',
            period: 'Jun 2019 - Sep 2019',
          },
        ],
      })
    },
}
</script>