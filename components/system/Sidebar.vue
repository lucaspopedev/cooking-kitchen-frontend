<template>
    <div class="relative flex min-h-screen">

        <!-- sidebar -->
        <div class="
                bg-red-800 
                w-56 
                rounded-r-3xl 
                space-y-6 
                absolute 
                inset-y-0 
                px-2
                left-0 
                transform
                -translate-x-full 
                md:relative md:-translate-x-0
                transition 
                duration-200 
                ease-in-out 
            " :class="{ 'hidden': showSidebar }">

            <nav class="mt-4">
                <span class="text-white p-4 text-2xl font-medium">Família Pope</span>

                <div class="text-white mt-4">
                    <a href="" class="flex items-center py-2 px-4 hover:bg-red-900 transition rounded-lg duration-300">

                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mr-2" fill="none" viewBox="0 0 24 24"
                            stroke="currentColor" stroke-width="2">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6" />
                        </svg>

                        <span>Dashboard</span>
                    </a>
                </div>

                <div class="text-white">
                    <a href=""
                        class="flex items-center py-2 mt-2 px-4 hover:bg-red-900 transition rounded-lg duration-300">

                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mr-2" fill="none" viewBox="0 0 24 24"
                            stroke="currentColor" stroke-width="2">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2m-3 7h3m-3 4h3m-6-4h.01M9 16h.01" />
                        </svg>

                        <span>Categorias</span>
                    </a>
                </div>

                <div class="text-white">
                    <a href=""
                        class="flex items-center py-2 mt-2 px-4 hover:bg-red-900 transition rounded-lg duration-300">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mr-2" fill="none" viewBox="0 0 24 24"
                            stroke="currentColor" stroke-width="2">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M12 6.253v13m0-13C10.832 5.477 9.246 5 7.5 5S4.168 5.477 3 6.253v13C4.168 18.477 5.754 18 7.5 18s3.332.477 4.5 1.253m0-13C13.168 5.477 14.754 5 16.5 5c1.747 0 3.332.477 4.5 1.253v13C19.832 18.477 18.247 18 16.5 18c-1.746 0-3.332.477-4.5 1.253" />
                        </svg>

                        <span>Receitas</span>
                    </a>
                </div>

                <div class="text-white">
                    <a href=""
                        class="flex items-center py-2 mt-2 px-4 hover:bg-red-900 transition rounded-lg duration-300">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mr-2" fill="none" viewBox="0 0 24 24"
                            stroke="currentColor" stroke-width="2">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M17 8h2a2 2 0 012 2v6a2 2 0 01-2 2h-2v4l-4-4H9a1.994 1.994 0 01-1.414-.586m0 0L11 14h4a2 2 0 002-2V6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2v4l.586-.586z" />
                        </svg>

                        <span>Dicas de cozinha</span>
                    </a>
                </div>

                <div class="text-white">
                    <a href=""
                        class="flex items-center py-2 mt-2 px-4 hover:bg-red-900 transition rounded-lg duration-300">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mr-2" fill="none" viewBox="0 0 24 24"
                            stroke="currentColor" stroke-width="2">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H7m10 0v-2c0-.656-.126-1.283-.356-1.857M7 20H2v-2a3 3 0 015.356-1.857M7 20v-2c0-.656.126-1.283.356-1.857m0 0a5.002 5.002 0 019.288 0M15 7a3 3 0 11-6 0 3 3 0 016 0zm6 3a2 2 0 11-4 0 2 2 0 014 0zM7 10a2 2 0 11-4 0 2 2 0 014 0z" />
                        </svg>
                        <span>Usuários</span>
                    </a>
                </div>

            </nav>

            <a class="absolute bottom-5 flex text-white items-center px-4 cursor-pointer">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mr-2" fill="none" viewBox="0 0 24 24"
                    stroke="currentColor" stroke-width="2">
                    <path stroke-linecap="round" stroke-linejoin="round"
                        d="M10 6H6a2 2 0 00-2 2v10a2 2 0 002 2h10a2 2 0 002-2v-4M14 4h6m0 0v6m0-6L10 14" />
                </svg>
                <span>Acessar site</span>
            </a>

        </div>

        <!-- Main Content -->
        <div class="flex-1">
            <!-- header -->
            <div class="bg-white border-b-2 px-4 py-4 font-semibold flex justify-between">
                <button @click="showSidebar = !showSidebar" class="text-red-900 font-extrabold">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24"
                        stroke="currentColor" stroke-width="2">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M4 6h16M4 12h8m-8 6h16" />
                    </svg>
                </button>

                <p class="text-red-900">Sair</p>
            </div>

            <!-- content -->
            <div class="p-8 text-red-800 font-extrabold">content title</div>
        </div>

    </div>
</template>

<script>
import { ref } from 'vue'
export default {
    name: "Sidebar",

    setup() {
        const showSidebar = ref(false);

        return {
            showSidebar,
        }
    }
}
</script>

<style>
</style>