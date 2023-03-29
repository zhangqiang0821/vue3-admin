<template>
  <div>
    <el-row :gutter="24">
      <el-col :span="24">
        <el-card shadow="hover">
          <template #header>
            <div class="clearfix">
              <span>基础信息</span>
            </div>
          </template>
          <div class="info">
            <div class="info-name">{{ name }}</div>
            <div class="info-desc">详情。。。。</div>
          </div>
        </el-card>
      </el-col>
    </el-row>
  </div>
</template>

<script setup lang="ts" name="user">
import { reactive, ref } from 'vue'
const ms_username = localStorage.getItem('ms_username')

const avatarImg = ref()
const name = ref(ms_username)
</script>

<style scoped></style>
