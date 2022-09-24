<template>
    <div clas="grid place-items-center">
        <div class="flex justify-center mt-6 px-5">
            <div class="w-full max-w-screen-lg flex flex-wrap justify-center rounded-lg md:border lg:border xl:border 2xl:border md:shadow-lg lg:shadow-lg xl:shadow-lg 2xl:shadow-lg">
              <div v-for="skill in skills" v-bind:key="skill.name" class="w-full m-4 border shadow-md md:m-0 lg:m-0 xl:m-0 md:shadow-none lg:shadow-none xl:shadow-none 2xl:shadow-none md:border-r-0 lg:border-r-0 xl:border-r-0 2xl:border-r-0 2xl:m-0 md:w-1/3 lg:w-1/3 xl:w-1/3 2xl:w-1/3 flex-none justify-center border-r p-4 text-center">
                <div class="bg-green-300 rounded-full h-20 w-20 mx-auto">&nbsp;</div>
                <div class="mt-4 font-bold">{{ skill.name }}</div>
                <div class="mt-4 text-purple-800">Frameworks and Tools I've used:</div>
                <div v-for="(framework, index) in skill.frameworks" v-bind:key="index">{{ framework }}</div>
                <div class="mt-4 text-purple-800" v-if="skill.languages">Languages I speak:</div>
                <div v-for="(language, index) in skill.languages" v-bind:key="index">{{ language }}</div>
              </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data: function () {
        return {
            skills: [
                {
                    name: "Frontend Development",
                    frameworks: [
                        "VueJS",
                        "AngularJS",
                        "Angular",
                        "Tailwind CSS",
                        "Bootstrap"
                    ]
                },
                {
                    name: "Backend Development",
                    frameworks: [
                        "ASP.NET",
                        "ASP.NET Core",
                        "Laravel",
                        "MS SQL",
                        "My SQL",
                        "Postgre SQL"
                    ],
                    languages: [
                        "C#",
                        "Javascript",
                        "Typescript",
                        "PHP",
                        "VB",
                        "Java",
                        "Swift"
                    ]
                },
                {
                    name: "Mobile Development",
                    frameworks: [
                        "Android Studio",
                        "Flutter",
                        "XCode"
                    ]
                }
            ]
        }
    },
}
</script>