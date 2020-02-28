<template>
    <nav class="navbar">
        <NavbarItem label="О приюте" url="/#about"></NavbarItem>
        <NavbarItem label="Наши животные" url="/#friends"></NavbarItem>
        <NavbarItem label="Помочь приюту" url="/#help"></NavbarItem>
        <NavbarItem label="Контакты" url="/#contacts"></NavbarItem>
    </nav>
</template>

<script>
    import NavbarItem from "./NavbarItem";
    export default {
        name: "Navbar",
        components: {
            NavbarItem
        }
    }
</script>

<style scoped lang="scss">
    .navbar {
        width: 463px;
        height: 31px;
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap ;
        position: relative;
        z-index: 1;
    }

</style>
