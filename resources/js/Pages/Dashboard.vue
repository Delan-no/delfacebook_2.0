<script setup>
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
import { Head } from '@inertiajs/vue3';
import { 
    HomeIcon, 
    ChatBubbleOvalLeftEllipsisIcon,  
    UserIcon,
    PlayCircleIcon,
    BellIcon,
    MapIcon } from "@heroicons/vue/24/outline";
import { Link } from '@inertiajs/vue3';
</script>

<template>
    <Head title="Acceuil" />

    <AuthenticatedLayout>
        <nav>
            <ul class="flex max-w-2xl mt-4 justify-around">
                <li class="flex flex-col items-center">
                    <Link :href="route('/profil')">
                        <HomeIcon class="h-8 w-8 text-blue-500" />
                    </Link>
                </li>
                <li class="flex flex-col items-center">
                    <a href="#">
                        <UserIcon class="h-8 w-8 text-blue-500" />
                    </a>
                </li>
                <li class="flex flex-col items-center">
                    <a href="#">
                        <ChatBubbleOvalLeftEllipsisIcon class="h-8 w-8 text-blue-500" />
                    </a>
                </li>
                <li class="flex flex-col items-center">
                    <a href="#">
                        <PlayCircleIcon class="h-8 w-8 text-blue-500" />
                    </a>
                </li>
                <li class="flex flex-col items-center">
                    <a href="#">
                        <BellIcon class="h-8 w-8 text-blue-500" />
                    </a>
                </li>
                <li class="flex flex-col items-center">
                    <a>
                        <MapIcon class="h-8 w-8 text-blue-500" />
                    </a>
                </li>
            </ul>
        </nav>
    </AuthenticatedLayout>
</template>
