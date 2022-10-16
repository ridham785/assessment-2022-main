<template >
    <div>
        
        <p v-for="(value,index) in Msgs" :key="index">{{ value}}</p>
        
    </div>
</template>

<script>
export default {
    name: 'Compontent2',
    props: [
        'Msgs'
    ]
        
        
        
    
}
</script>