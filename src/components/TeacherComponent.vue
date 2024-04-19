<template>
    <h2>Teacher name is : {{ name }}</h2>
</template>

<script>
export default {
    name: 'TeacherComponent',
    props: {
        name: String
    }
};
</script>