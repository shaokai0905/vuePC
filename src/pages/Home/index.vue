<template>
    <div>
        <TypeNav/>
        <ListContainer/>
        <TodayRecommend/>
        <Rank/>
        <Like></Like>
        <Floor></Floor>
        <Brand></Brand>
    </div>
</template>

<script>
import ListContainer from './ListContainer'
import TodayRecommend from './TodayRecommend'
import Brand from './Brand/Brand'
import Floor from './Floor/Floor'
import Like from './Like/Like'
import Rank from './Rank/Rank'
export default {
    name: '',
    components:{
        ListContainer,
        TodayRecommend,
        Brand,
        Floor,
        Like,
        Rank
    }
}
</script>

<style scoped>

</style>
