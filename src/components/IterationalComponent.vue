<script setup>
import { ref } from 'vue'

const people = ref(['Asfar', 'Zain', 'Ali'])
const books = [
  {
    id: '1',
    title: 'To Kill a Mockingbird',
    genre: 'Fiction',
    author: 'Harper Lee'
  },
  {
    id: '2',
    title: '1984',
    genre: 'Dystopian',
    author: 'George Orwell'
  },
  {
    id: '3',
    title: 'The Great Gatsby',
    genre: 'Classic',
    author: 'F. Scott Fitzgerald'
  },
  {
    id: '4',
    title: 'The Catcher in the Rye',
    genre: 'Fiction',
    author: 'J.D. Salinger'
  },
  {
    id: '5',
    title: 'Moby-Dick',
    genre: 'Adventure',
    author: 'Herman Melville'
  },
  {
    id: '6',
    title: 'Pride and Prejudice',
    genre: 'Romance',
    author: 'Jane Austen'
  },
  {
    id: '7',
    title: 'The Lord of the Rings',
    genre: 'Fantasy',
    author: 'J.R.R. Tolkien'
  },
  {
    id: '8',
    title: 'The Hobbit',
    genre: 'Fantasy',
    author: 'J.R.R. Tolkien'
  },
  {
    id: '9',
    title: "Harry Potter and the Sorcerer's Stone",
    genre: 'Fantasy',
    author: 'J.K. Rowling'
  },
  {
    id: '10',
    title: 'The Da Vinci Code',
    genre: 'Mystery',
    author: 'Dan Brown'
  }
]
</script>
<template>
  <h1 v-for="(person, index) in people" :key="index">{{ person }}</h1>
  <ul v-for="({ id, title, genre, author }, i) in books" :key="i">
    <p>Book {{ id }}</p>
    <li>Title: {{ title }}</li>
    <li>Genre: {{ genre }}</li>
    <li>Author: {{ author }}</li>
  </ul>
</template>
