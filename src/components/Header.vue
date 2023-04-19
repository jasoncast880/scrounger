<template>
    <header>
        <h1>{{ title }}</h1>
        <Button text = "Add Task" color="green" />
    </header>
    <br>
    <body>
        <p><i>Another mans trash is your treasure!</i></p>
    </body>
</template>

<script>
    import Button from './Button'

export default{
    name: 'Header',
    props: {
        title: String,
        headerText: String,
    },
    components: {
        Button
    }    
}
</script>

<style scoped>
    header{
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin: bottom 20px;
    }

</style>