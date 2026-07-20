<script setup lang="ts">
defineProps<{
  student: {
    id: number
    studentId: string
    name: string
    surname: string
    gpa: number
    image: string
    penamount: number
    description: string
  }
}>()
</script>

<template>
  <div class="student-card">
    <h2>{{ student.name }} {{ student.surname }}</h2>
    <p>GPA: {{ student.gpa }}</p>
  </div>
</template>

<style scoped>
.student-card {
  padding: 20px;
  width: 250px;
  cursor: pointer;
  border: 1px solid #39495c;
  margin-bottom: 18px;
  border-radius: 8px;
}
</style>