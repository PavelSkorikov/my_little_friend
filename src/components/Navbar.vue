<template>
    <nav class="navbar">
        <NavbarItem label="About the shelter" url="/#about"></NavbarItem>
        <NavbarItem label="Our pets" url="/#friends"></NavbarItem>
        <NavbarItem label="To help the shelter" url="/#help"></NavbarItem>
        <NavbarItem label="Contacts" url="/#contacts"></NavbarItem>
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
