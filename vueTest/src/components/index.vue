<template>
    <div>
        <p>
             {{title}}
        </p>
        <p>
             {{msg}}
        </p>
      
    </div>
</template>

<script>
export default {
    data(){
        return {
            title:'i love u'
        }
    },
    props:['msg']
}
</script>

<style>

</style>

