<template>
  <div>
    <p>普通按钮</p>
    <el-row>
      <el-button>默认按钮</el-button>
      <el-button type="primary">主要按钮主要按钮主要按钮主要按钮</el-button>
      <el-button type="success">成功按钮</el-button>
      <el-button type="info">信息按钮</el-button>
      <el-button type="warning">警告按钮</el-button>
      <el-button type="danger">危险按钮</el-button>
    </el-row>
    <br>
    <p>带图标</p>
    <el-row>
      <el-button>默认按钮</el-button>
      <el-button :loading="true" type="primary">普通按钮</el-button>
      <el-button icon="el-icon-folder-delete" type="primary">成功按钮</el-button>
      <el-button icon="el-icon-folder-delete" type="primary"></el-button>
    </el-row>
    <br>
    <p>文字按钮</p>
    <el-row>
      <el-button type="text">文字按钮</el-button>
      <el-button type="text" disabled>文字按钮</el-button>
    </el-row>
    <br>
    <el-row>
      <el-button round>圆角按钮</el-button>
      <el-button type="primary" round>主要按钮</el-button>
      <el-button type="success" round>成功按钮</el-button>
      <el-button type="info" round>信息按钮</el-button>
      <el-button type="warning" round>警告按钮</el-button>
      <el-button type="danger" round>危险按钮</el-button>
    </el-row>
    <br>
    <el-row>
      <el-button icon="el-icon-search" circle></el-button>
      <el-button type="primary" icon="el-icon-edit" circle></el-button>
      <el-button type="success" icon="el-icon-check" circle></el-button>
      <el-button type="info" icon="el-icon-message" circle></el-button>
      <el-button type="warning" icon="el-icon-star-off" circle></el-button>
      <el-button type="danger" icon="el-icon-delete" circle></el-button>
    </el-row>
  </div>
</template>
