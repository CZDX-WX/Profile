<template>
    <div class="collapse">
        <el-collapse v-model="activeNames" @change="handleChange" background-color="#fffdf4" accordion>
            <el-collapse-item name="1">
                <template #title>
                    <el-icon class="icon">
                        <Briefcase />
                    </el-icon>
                    <info-filled />
                    Education Background
                </template>
                <el-table :data="schoolData" size="small">
                    <el-table-column prop="name" label="校名" width="180" stripe />
                    <el-table-column prop="time" label="时间" />
                </el-table>
            </el-collapse-item>

            <el-collapse-item name="2">
                <template #title>
                    <el-icon class="icon">
                        <Briefcase />
                    </el-icon>
                    <info-filled />
                    Certificate
                </template>
                <el-table :data="certificateData" size="small" stripe>
                    <el-table-column prop="name" label="证书" width="180" />
                    <el-table-column prop="date" label="时间" />
                </el-table>
            </el-collapse-item>

            <el-collapse-item name="3">
                <template #title>
                    <el-icon class="icon">
                        <Briefcase />
                    </el-icon>
                    <info-filled />
                    Skill Stack
                </template>
                <el-table :data="skillData" size="small" stripe>
                    <el-table-column prop="name" label="技能" width="180" />
                    <el-table-column prop="frame" label="相关技术栈" />
                </el-table>
            </el-collapse-item>

            <el-collapse-item name="4">
                <template #title>
                    <el-icon class="icon">
                        <Briefcase />
                    </el-icon>
                    <info-filled />
                    Work Experience
                </template>
                <el-table :data="workData" size="small" stripe>
                    <el-table-column prop="name" label="公司" width="180" />
                    <el-table-column prop="address" label="地址" />
                    <el-table-column prop="job" label="岗位" />
                </el-table>
            </el-collapse-item>

            <el-collapse-item name="5">
                <template #title>
                    <el-icon class="icon">
                        <Briefcase />
                    </el-icon>
                    <info-filled />
                    Project Experience
                </template>
                <el-table :data="projectionData" size="small" stripe>
                    <el-table-column prop="name" label="项目名" width="180" />
                    <el-table-column prop="function" label="需求" />
                    <el-table-column prop="task" label="负责任务" />
                </el-table>
            </el-collapse-item>


        </el-collapse>
    </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue';
import { schoolData, certificateData, skillData, workData, projectionData } from '@/assets/static/Data';



const activeNames = ref(['1'])
const handleChange = (val: string[]) => {
    console.log(val)
}




</script>


<style scoped>

.collapse {
    padding: 5px;
    margin: auto;
    width: 100%;
    height: 100%;
    font-family: inherit;
    background: inherit;
}

.icon {
    font-size: 24px;
    /* 设置图标大小 */
    color: #007aff;
    /* 设置图标颜色 */
}
</style>