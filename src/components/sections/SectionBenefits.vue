<template lang="pug">
.section-why
  .section-home.section-home-benefits: .section-home__container
    .section-home__header Why Use Cosmos?
    .section-home__main
      .cosmos-panels
        .cosmos-panel
          .cosmos-panel__image
            img.cosmos-panel__img(
              src="images/diagrams/panel-interoperability.png" alt="interoperability")
          .cosmos-panel__text
            .cosmos-panel__title Interoperable
            .cosmos-panel__body The Cosmos Network is built to allow many independent blockchains &ndash; public and private &ndash; to communicate and exchange value with one another.
            .cosmos-panel__action
              a(href="/docs/resources/whitepaper.html#inter-blockchain-communication-ibc") Interblockchain Comms &rsaquo;

        .cosmos-panel
          .cosmos-panel__image
            img.cosmos-panel__img(
              src="images/diagrams/panel-scalability.png" alt="scalability")
          .cosmos-panel__text
            .cosmos-panel__title Scalable
            .cosmos-panel__body By leveraging interoperability and Tendermint’s Proof-of-Stake algorithm, Cosmos provides unprecedented levels of scalability for blockchain networks.
            .cosmos-panel__action
              a(href="/docs/resources/whitepaper.html#horizontal-scaling") Scaling Cosmos &rsaquo;

        .cosmos-panel
          .cosmos-panel__image
            img.cosmos-panel__img(
              src="images/diagrams/panel-developer-friendly.png" alt="developer friendly")
          .cosmos-panel__text
            .cosmos-panel__title Developer Friendly
            .cosmos-panel__body Cosmos was designed with developers in mind. Thanks to Tendermint’s Application Blockchain Interface, it’s easy to build blockchains in any programming language.
            .cosmos-panel__action
              a(href="/docs/sdk/overview.html") Cosmos for Developers &rsaquo;
</template>

<script>
export default {
  name: "section-benefits"
}
</script>

<style lang="stylus">
@require '~variables'
.cosmos-panels
  margin 0 -1rem

.cosmos-panel
  background var(--app-fg)
  display flex
  flex-flow column nowrap
  margin 1rem

  &:first-child
    margin-top 0

  &:last-child
    margin-bottom 0

.cosmos-panel__title
.cosmos-panel__body
.cosmos-panel__action
  padding 1rem

.cosmos-panel__title + .cosmos-panel__body
  padding-top 0

.cosmos-panel__body + .cosmos-panel__action
  padding-top 0

.cosmos-panel__title
  color var(--bright)
  font-size h2

.cosmos-panel__img
  width 100%

.cosmos-panel__action
  display block

@media screen and (min-width: 768px)
  .cosmos-panel
    flex-flow row nowrap

  .cosmos-panel__image
    flex 1

  .cosmos-panel__text
    flex 2

  .cosmos-panel__title
  .cosmos-panel__body
  .cosmos-panel__action
    padding 1.5rem

@media screen and (min-width: 1024px)
  .cosmos-panels
    display flex
    flex-flow row nowrap

  .cosmos-panel
    flex 1
    flex-flow column nowrap
    display block
    &:first-child
    &:last-child
      margin 1rem

  .cosmos-panel__text
    display flex
    flex-flow column

  .cosmos-panel__body
    flex 1
    height 11rem
</style>
