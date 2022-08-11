<template>
    <div class="desktop flex flex-col w-screen h-screen overflow-hidden">
        <Workspace />
        <TaskBar />
        <StartMenu />
        <Calendar />
        <NotificationCenter />
    </div>
</template>

<script>
import Workspace from './Workspace'
import TaskBar from './TaskBar'
import StartMenu from './StartMenu'
import NotificationCenter from './NotificationCenter'
import Calendar from './Calendar'

export default {
    name: 'Desktop',
    components: {
        Workspace,
        TaskBar,
        StartMenu,
        Calendar,
        NotificationCenter
    }
}
</script>

<style lang="scss" scoped>
.desktop {
    background-image: url('../assets/wallpapers/light.jpg');
    background-position: center;
    background-size: cover;
}

.dark {
    .desktop {
        background-image: url('../assets/wallpapers/dark.jpg');
    }
}
</style>