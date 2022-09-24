<template>
    <div class="w-full grid place-items-center mt-20">
        <div class="text-2xl font-bold max-w-screen-lg">My Recent Projects</div>
        <div class="mt-4 text-center px-5">Here are a few of my projects that I've work on.</div>
        <div class="grid mx-5 xl:mx-0 2xl:mx-0 md:grid-cols-2 lg:grid-cols-2 xl:grid-cols-2 2xl:grid-cols-2 gap-4 max-w-screen-lg mt-6">
            <div v-for="(project, index) in projects" v-bind:key="index" class="bg-purple-600 h-auto lg:h-60 xl:h-60 2xl:h-60 rounded-xl text-center text-white p-5 shadow-lg">
                <div class="text-xl my-4 uppercase font-semibold tracking-widest text-green-300">{{ project.name }}</div>
                <div class="text-sm tracking-widest">{{ project.description }}</div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data: function () {
        return {
            projects: [
                {
                    name: "Contentree",
                    description: "This is a content collection which helps the users to find the content they are looking for. It is build with ASP.NET MVC framework and AngularJS for the frontend. We are also using MS SQL Server for the database."
                },
                {
                    name: "eDoc v11",
                    description: "This is a transcription platform used by the clients where the doctor/author can upload/record their dictation and can be process by their internal team or they can be outsourced. The application is multiplatform which the users can access it via browser or mobile phones (Android/iOS)."
                },
                {
                    name: "Inhouse Speech Recognition Automation",
                    description: "This is a automation that convert the speech into a text using the Azure Speech SDK. This is integrated with the inhouse applications of the company. It has queueing process to make sure all audios can be processed and track all those failed convertion."
                },
                {
                    name: "Quality Assurance Scoring Software",
                    description: "This is a desktop application that records all the audited score of the transcriptionist of the company. The company also used this to track the performance of their transcriptionists. The application is integrated with Microsoft Interop for Word Application."
                },
                {
                    name: "Human Resource Information System",
                    description: "This is a web application that manage the record and payroll of the employees of the company. It is build in ASP.NET Web Forms and MS SQL for the database."
                },
                {
                    name: "Human Edge",
                    description: "This is a interprise employee management that handles the employees information including daily time record and payroll. It has a multiple application for the users type. It is build in ASP.NET Classic and ASP.NET MVC. We are also using MS SQL for the database."
                }
            ]
        }
    },
}
</script>

<style>

</style>