<template>
    <div class="greadheader"
    :style="'width:'+width + ';background-color:'+headerColor+ ';'">
        <div v-for="field in fields"
            :style="styleClass(field)">
            {{field.name}}
        </div>
    </div>
</template>

<script>
import gridjs from './grid.js';

export default {
    props: gridjs.props,
    methods: gridjs.methods,
    computed: gridjs.computed,
    watch: gridjs.watch
}
</script>