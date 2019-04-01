<template lang="pug">
  .wrapper
    header.header
      .container.header__container
        .header__col.header__col_left
          .header__user-avatar
            img(src="../images/content/uMmrjh-M3HA.jpg" alt="User Photo").header__user-avatar-pic
          .header__user-name Дарья Марченко
          .header__desc Панель администрирования
        .header__col.header__col_right
          a(href="#").header__link-close Выйти

    nav.nav
      .container.nav__container
        ul.nav__list
          li.nav__item
            a(href="#").nav__link Обо мне
          li.nav__item
            a(href="#").nav__link Работы
          li.nav__item
            a(href="#").nav__link Отзывы
    
    .main-content
      .section.about
        .container.about__container
          .about__top
            h1.title.about__title Блок «Обо мне»  
            button(type="button").btn.about__top-btn Добавить группу

          .about__content

            .cards
              ul.cards__list
                li.cards__item
                  .cards__top
                    label.cards__form-block
                      input(type="text" placeholder="Название новой группы").cards__input
                    .cards__top-btns
                      button(type="button").cards__top-btn-approve
                      button(type="button").cards__top-btn-remove
                  .cards__main-content
                  .cards__bottom
                    label.cards__form-block
                      input(type="text" placeholder="Новый навык").cards__input
                    label.cards__form-block.cards__form-block_percent
                      input(type="text" placeholder="100").cards__input.card__input-percent
                      span.card__input-percent %
                    button(type="button").btn.cards__botom-btn
                    
                
                li.cards__item
                  .cards__top
                    label.cards__form-block
                      input(type="text" placeholder="Название новой группы" value="Workflow").cards__input
                    .cards__top-btns
                      button(type="button").cards__top-btn-approve
                      button(type="button").cards__top-btn-remove

                  .cards__main-content
                    table.cards__table
                      tr.cards__row
                        td.cards__cell
                          span.cards__cell-name GIT
                        td.cards__cell
                          .cards__cell-percent
                            span.cards__input.card__input-percent.card__input-percent-table 100
                            span.card__input-percent %
                        td.cards__cell
                          .cards__cell-btns
                            button(type="button").cards__cell-btn-edit
                            button(type="button").cards__cell-btn-delete
                          
                      tr.cards__row
                        td.cards__cell
                          span.cards__cell-name Terminal
                        td.cards__cell
                          .cards__cell-percent
                            span.cards__input.card__input-percent.card__input-percent-table 90
                            span.card__input-percent %
                        td.cards__cell
                          .cards__cell-btns
                            button(type="button").cards__cell-btn-edit
                            button(type="button").cards__cell-btn-delete

                      tr.cards__row
                        td.cards__cell
                          span.cards__cell-name Gulp
                        td.cards__cell
                          .cards__cell-percent
                            span.cards__input.card__input-percent.card__input-percent-table 80
                            span.card__input-percent %
                        td.cards__cell
                          .cards__cell-btns
                            button(type="button").cards__cell-btn-edit
                            button(type="button").cards__cell-btn-delete

                      tr.cards__row
                        td.cards__cell
                          span.cards__cell-name Webpack
                        td.cards__cell
                          .cards__cell-percent
                            span.cards__input.card__input-percent.card__input-percent-table 85
                            span.card__input-percent %
                        td.cards__cell
                          .cards__cell-btns
                            button(type="button").cards__cell-btn-edit
                            button(type="button").cards__cell-btn-delete

                    


                  .cards__bottom
                    label.cards__form-block
                      input(type="text" placeholder="Новый навык").cards__input
                    label.cards__form-block.cards__form-block_percent
                      input(type="text" placeholder="100").cards__input.card__input-percent
                      span.card__input-percent %
                    button(type="button").btn.cards__botom-btn 


                li.cards__item
                  .cards__top
                    label.cards__form-block
                      input(type="text" placeholder="Название новой группы" value="Workflow").cards__input
                    .cards__top-btns
                      button(type="button").cards__top-btn-approve
                      button(type="button").cards__top-btn-remove

                  .cards__main-content
                    table.cards__table
                      tr.cards__row
                        td.cards__cell
                          span.cards__cell-name GIT
                        td.cards__cell
                          .cards__cell-percent
                            span.cards__input.card__input-percent.card__input-percent-table 100
                            span.card__input-percent %
                        td.cards__cell
                          .cards__cell-btns
                            button(type="button").cards__cell-btn-edit
                            button(type="button").cards__cell-btn-delete
                          
                      tr.cards__row
                        td.cards__cell
                          span.cards__cell-name Terminal
                        td.cards__cell
                          .cards__cell-percent
                            span.cards__input.card__input-percent.card__input-percent-table 90
                            span.card__input-percent %
                        td.cards__cell
                          .cards__cell-btns
                            button(type="button").cards__cell-btn-edit
                            button(type="button").cards__cell-btn-delete

                      tr.cards__row
                        td.cards__cell
                          span.cards__cell-name Gulp
                        td.cards__cell
                          .cards__cell-percent
                            span.cards__input.card__input-percent.card__input-percent-table 80
                            span.card__input-percent %
                        td.cards__cell
                          .cards__cell-btns
                            button(type="button").cards__cell-btn-edit
                            button(type="button").cards__cell-btn-delete

                      tr.cards__row
                        td.cards__cell
                          span.cards__cell-name Webpack
                        td.cards__cell
                          .cards__cell-percent
                            span.cards__input.card__input-percent.card__input-percent-table 85
                            span.card__input-percent %
                        td.cards__cell
                          .cards__cell-btns
                            button(type="button").cards__cell-btn-edit
                            button(type="button").cards__cell-btn-delete

                    


                  .cards__bottom
                    label.cards__form-block
                      input(type="text" placeholder="Новый навык").cards__input
                    label.cards__form-block.cards__form-block_percent
                      input(type="text" placeholder="100").cards__input.card__input-percent
                      span.card__input-percent %
                    button(type="button").btn.cards__botom-btn 






    






</template>


<style lang="postcss">
@import url('https://fonts.googleapis.com/css?family=Open+Sans:300,400,600,700,800');
@import "normalize.css";
@import "../styles/mixins.pcss";
@import "../styles/layout/base.pcss";
@import "../styles/admin/header.pcss";
@import "../styles/admin/nav.pcss";
@import "../styles/admin/main-content.pcss";
@import "../styles/admin/about.pcss";
@import "../styles/admin/cards.pcss";
</style>