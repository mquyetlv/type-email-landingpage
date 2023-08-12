<template>
  <div class="header fixed z-[999]">
    <div class="container-layout w-100 md:container mx-auto flex items-center justify-between h-[80px] bg-primary-color">
      <div class="flex items-center">
        <img src="../assets/images/logo.png" alt="Logo" class="mr-1" />
        <img src="../assets/images/type-email.png" alt="Logo text" />
      </div>

      <div>
        <ul class="menu">
          <li class="menu-item">Home</li>
          <li class="menu-item active">Pricing</li>
          <li class="menu-item">Resource</li>
          <li class="menu-item">Support</li>
        </ul>
      </div>

      <button class="btn btn-small">Login</button>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
.header {
  background-color: var(--primary-bg-color);
  top: 0;
  left: 0;
  right: 0;
}

.menu {
  display: flex;
  color: var(--second-white);
}

.menu-item {
  position: relative;
}

.menu-item:hover {
  cursor: pointer;
  color: var(--primary-white);
}
.menu-item + .menu-item {
  margin-left: 36px;
}

.menu-item.active {
  color: var(--primary-white);
}

.menu-item.active::before {
  content: "";
  display: block;
  width: 12px;
  height: 2px;
  position: absolute;
  bottom: 0;
  left: 0;
  background: var(--linear-gradient);
}
</style>
