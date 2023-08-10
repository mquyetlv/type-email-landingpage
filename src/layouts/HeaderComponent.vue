<template>
  <div class="w-100 md:container fixed mx-auto flex items-center justify-between h-[80px] inset-0 bg-primary-color z-[999]">
    <div class="flex items-center">
      <img src="../assets/images/logo.png" alt="Logo" class="mr-1">
      <img src="../assets/images/type-email.png" alt="Logo text">
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
</template>

<script setup></script>

<style scoped>
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
    content: '';
    display: block;
    width: 12px;
    height: 2px;
    position: absolute;
    bottom: 0;
    left: 0;
    background: var(--linear-gradient);
  }
</style>
