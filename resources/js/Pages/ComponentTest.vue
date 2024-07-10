<script setup>
import { reactive, ref } from 'vue'
import GuestLayout from '@/Layouts/GuestLayout.vue'
import Label from '@/Components/InputLabel.vue'
import Input from '@/Components/TextInput.vue'

const model = ref('')
function output(){
    console.log(model.value)
}

</script>

<template>
    <GuestLayout>
    <Label value="件名">タイトル</Label>
    <Input modelValue="初期値が入ります。" v-model="model" @input="output"></Input>
    </GuestLayout>
</template>