<template>
    <div>
        <input v-model="message" autofocus/>
        <div>{{ message }}</div>
        <div>Open browser's developer console to see the calculation log</div>
        <ul>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
            <li>char count: {{ messageCharCount }}</li>
        </ul>
    </div>
</template>

<script lang="ts">
    import {Component, Vue} from 'vue-property-decorator'

    @Component({})
    export default class App extends Vue {
        message: string = 'change me'

        get messageCharCount(): number {
            const now = new Date().getTime()
            console.log('calculate char count at ' + now)
            return this.message.length
        }
    }
</script>
