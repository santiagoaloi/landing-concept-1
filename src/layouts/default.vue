<template>
  <div>
    <GSystemBar />
    <GAppBar />
    <VMain scrollable>
      <BlurBackground />
      <SJContainer>
        <RouterView v-slot="{ Component }">
          <template v-if="Component">
            <VFadeTransition hide-on-leave>
              <VContainer fluid>
                <Component :is="Component" />
              </VContainer>
            </VFadeTransition>
          </template>
        </RouterView>
      </SJContainer>
    </VMain>
  </div>
</template>
