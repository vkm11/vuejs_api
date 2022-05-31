<template>
    <h1>Call API</h1>
</template>

<script>
import axios from 'axios';
export default{ 
    name: "App",
    data()
    {
        return{
            list:[]
        }
    },
    async mounted()
    {
        let result = await axios.get("https://reqres.in/api/users?page=1");
        console.log("Api data",result.data.data)
    }
};
</script>