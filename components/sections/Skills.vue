<template>
    <section class="section">
        <h2 class="section__title">Skills</h2>

        <div class="skills-container" v-for="item in skills">
            <h3>{{item.title}}</h3>
            <ul class="skills-list">
                <li class="skills_list__item" v-for="skill in item.content">{{skill}}</li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: "Skills",
    data() {
        return {
            skills: [
                {
                    title: "JavaScript",
                    content: [
                        "ES8","VueJS + Vuex", "NuxtJS  Praca z REST API", "end-to-end tests with CypressJS "  ,"DOM Manipulations"
                    ]
                },
                  {
                    title: "JavaScript",
                    content: [
                        "ES8","VueJS + Vuex", "NuxtJS  Praca z REST API", "end-to-end tests with CypressJS "  ,"DOM Manipulations"
                    ]
                },
                  {
                    title: "JavaScript",
                    content: [
                        "ES8","VueJS + Vuex", "NuxtJS  Praca z REST API", "end-to-end tests with CypressJS ",  "DOM Manipulations"
                    ]
                },
                  {
                    title: "JavaScript",
                    content: [
                        "ES8","VueJS + Vuex", "NuxtJS  Praca z REST API", "end-to-end tests with CypressJS " , "DOM Manipulations"
                    ]
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.section {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.skills-container { 
    width: 75%;
    display: flex;
    justify-content: center;
    flex-flow: column wrap;
}

.skills-container:not(:first-child) {
    margin-top: 2rem;
}

.skills-list {
    display: flex;
    list-style: none;
    margin-top: 1rem;
}

.skills_list__item {
    margin-left: $s1;
}
</style>