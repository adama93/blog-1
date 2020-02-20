<template>
    <div>
        <table>
        <tr>{{ article.title }}</tr>
        <tr>{{ article.body }}</tr>
        <tr>{{ article.author }}</tr>
        
         <div v-for="commentaire in article.comment" :key="commentaire.title">
            <tr>{{commentaire.title}}</tr>
        <tr>{{commentaire.body}}</tr>
        
        </div>
        </table>
    </div>
</template>

<script>
export default {
    props: 
        ['article','comment']
};
</script>