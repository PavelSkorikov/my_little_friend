<template>
    <nav class="navbar">
        <NavbarItem label="About the shelter" url="About"></NavbarItem>
        <NavbarItem label="Our pets" url="Friends"></NavbarItem>
        <NavbarItem label="To help the shelter" url="Help"></NavbarItem>
        <NavbarItem label="Contacts" url="Contacts"></NavbarItem>
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
