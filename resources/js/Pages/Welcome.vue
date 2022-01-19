<template>
    <layout>
        <div>
            <p>this is a welcome page: {{ foo }}</p>
        </div>
    </layout>
</template>

<script>
    import Layout from '@/Shared/Layout'
    export default {
        props: ['foo'],
            components: {
                Layout,
            },
        }
</script>
