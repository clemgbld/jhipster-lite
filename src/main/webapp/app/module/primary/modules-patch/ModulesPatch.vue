<template src="./ModulesPatch.html"></template>

<script lang="ts" src="./ModulesPatch.component.ts"></script>

<style lang="scss">
.jhipster-modules {
  color: var(--jhlite-global-color-text);
}

.jhipster-modules-list {
  flex-grow: 1;
  display: flex;
  flex-direction: column;

  &--categories {
    overflow-y: auto;
    flex-grow: 1;
    padding: 0 15px;
  }
}

.jhipster-modules-filters {
  margin: 15px 0;
  padding: 0 15px;
  height: 40px;
  display: flex;
  align-items: center;

  &--tags {
    margin-right: 10px;
  }

  &--filter {
    font-size: 1.4em;
    border: 1px solid $jhipster-lite-line-color;
    border-radius: $jhipster-lite-box-radius;
    padding: 0 10px;
    flex-grow: 1;
  }

  &--displayed-modules-count {
    margin-left: 15px;
    background-color: $jhipster-lite-primary-color;
    padding: 3px 1em;
    border-radius: 1em;
    color: #ffffff;
  }
}

.jhipster-module-category {
  &--name {
    font-size: 1.4em;
    font-weight: 800;
  }
}

.jhipster-module {
  border: 1px solid $jhipster-lite-line-color;
  border-radius: $jhipster-lite-box-radius;
  margin-bottom: 10px;
  display: flex;

  &.selected {
    background-color: $jhipster-lite-primary-color;
    color: var(--jhlite-white);
  }

  &--content {
    cursor: pointer;
    flex-grow: 1;
    padding: 5px 10px;
  }

  &--content.not-selected {
    display: flex;
  }

  &--content.applied {
    background-color: $jhipster-lite-applied-module-color;
  }

  &--tags.not-selected,
  &--description.not-selected {
    display: none;
  }

  &--tags.selected {
    display: flex;
    margin: 5px 0;
  }

  &--description.selected {
    display: block;
  }

  &--tag {
    background-color: $jhipster-lite-secondary-color;
    font-style: italic;
    margin-right: 7px;
    padding: 0 0.5em;
    border-radius: 1em;
  }

  &--slug {
    font-weight: bold;
  }

  &--apply-button {
    background-color: transparent;
    border: 0;
    border-left: 1px solid $jhipster-lite-line-color;
    padding: 0 10px;
    color: $jhipster-lite-primary-input-color;
    font-weight: bold;
    font-size: 1.5em;
  }

  &--apply-button:disabled {
    color: $jhipster-lite-disabled-color;
  }
}
</style>
