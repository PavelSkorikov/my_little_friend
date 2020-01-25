<template>
    <nav class="navbar">
        <NavbarItem label="About the shelter"></NavbarItem>
        <NavbarItem label="Our pets"></NavbarItem>
        <NavbarItem label="To help the shelter"></NavbarItem>
        <NavbarItem label="Contacts"></NavbarItem>
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
        max-width: 463px;
        margin-left: 132px;
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap ;
        position: relative;
        z-index: 1;
    }

</style>
