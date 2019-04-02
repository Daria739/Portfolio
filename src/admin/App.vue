<template lang="pug">
  .wrapper
    section.login
      .login__content
       
        form.login__form
          button(type="button").login__form-close
          h1.login__form-title Авторизация
          .login__row
            label.login__form-block
              span.login__form-block-title Логин
              .login__form-block-container
                .login__input-user-pic
                input(type="text" placeholder="Terminator__2000" required).login__input
          .login__row
            label.login__form-block
              span.login__form-block-title Пароль
              .login__form-block-container
                .login__input-password-pic
                input(type="text" placeholder="••••••••" required).login__input
          .login__btn
            button(type="submit").login__btn-submit Отправить

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
      section.works
        .container.works__container
          h1.title.works__title Блок «Работы»
          .works__content
            ul.works__content-list

              li.works__content-item.works__content-item_new-card
                button(type="button").works__content-item_new-card-btn
                  span.works__content-item_new-card-title Добавить работу

              li.works__content-item
                .works__content-top
                  img(src="../images/content/preview-1.jpg" alt="Preview").works__content-top-pic
                  ul.works__tags-list
                    li.works__tags-item HTML
                    li.works__tags-item CSS
                    li.works__tags-item Javascript

                .works__desc
                  h3.title.works__title-desc Сайт школы образования
                  p.works__info Эта девушка проходила обучение веб-разработке не где-то, а в LoftSchool! 4,5 месяца только самых тяжелый испытаний и бессонных ночей!
                  a(href="#").works__link http://loftschool.ru
                  .works__btns
                    button(type="button").btn.btn-edit Править
                    button(type="button").btn.btn-delete Удалить
              li.works__content-item
                .works__content-top
                  img(src="../images/content/preview-1.jpg" alt="Preview").works__content-top-pic
                  ul.works__tags-list
                    li.works__tags-item HTML
                    li.works__tags-item CSS
                    li.works__tags-item Javascript

                .works__desc
                  h3.title.works__title-desc Сайт школы образования
                  p.works__info Эта девушка проходила обучение веб-разработке не где-то, а в LoftSchool! 4,5 месяца только самых тяжелый испытаний и бессонных ночей!
                  a(href="#").works__link http://loftschool.ru
                  .works__btns
                    button(type="button").btn.btn-edit Править
                    button(type="button").btn.btn-delete Удалить
              li.works__content-item
                .works__content-top
                  img(src="../images/content/preview-1.jpg" alt="Preview").works__content-top-pic
                  ul.works__tags-list
                    li.works__tags-item HTML
                    li.works__tags-item CSS
                    li.works__tags-item Javascript

                .works__desc
                  h3.title.works__title-desc Сайт школы образования
                  p.works__info Эта девушка проходила обучение веб-разработке не где-то, а в LoftSchool! 4,5 месяца только самых тяжелый испытаний и бессонных ночей!
                  a(href="#").works__link http://loftschool.ru
                  .works__btns
                    button(type="button").btn.btn-edit Править
                    button(type="button").btn.btn-delete Удалить
              li.works__content-item
                .works__content-top
                  img(src="../images/content/preview-1.jpg" alt="Preview").works__content-top-pic
                  ul.works__tags-list
                    li.works__tags-item HTML
                    li.works__tags-item CSS
                    li.works__tags-item Javascript

                .works__desc
                  h3.title.works__title-desc Сайт школы образования
                  p.works__info Эта девушка проходила обучение веб-разработке не где-то, а в LoftSchool! 4,5 месяца только самых тяжелый испытаний и бессонных ночей!
                  a(href="#").works__link http://loftschool.ru
                  .works__btns
                    button(type="button").btn.btn-edit Править
                    button(type="button").btn.btn-delete Удалить
      section.reviews
        .container.reviews__container
          h1.title.reviews__title Блок «Отзывы»
          .reviews__new
            h2.title.reviews__new-title Новый отзыв
            form.reviews__form
              .form__main-content
                .form__col.form__col_left
                  .form__user-photo
                  button(type="button").form__user-add-photo Добавить фото

                .form__col.form__col_right
                  .form__row
                    label.form__block
                      span.form__block-title.form__block-title_user Имя автора
                      .form__block-container
                        input(type="text" placeholder="Дмитрий Ковальчук" required).form__input

                    label.form__block
                      span.form__block-title Титул автора
                      .form__block-container
                        input(type="text" placeholder="Основатель LoftSchool" required).form__input

                  .form__row
                  label.form__block.form__block_textarea
                    span.form__block-title.form__block-title_textarea Сообщение к письму
                    .form__block-container.form__block-container_textarea
                      textarea(placeholder="Эта девушка проходила обучение веб-разработке не где-то, а в LoftSchool! 4,5 месяца только самых тяжелых испытаний и бессонных ночей!").form__input_textarea
              .form__btns
                button(type="button").form__btn-cancel Отмена
                button(type="button").form__btn-save Сохранить
            
          ul.reviews__list
            li.reviews__item.reviews__item_new
              button(type="button").reviews__item_new-btn
                span.reviews__item_new-title Добавить отзыв

            li.reviews__item
              .reviews__item-top
                .reviews__author-img
                  img(src="../images/content/Vladimir.jpg" alt="Vladimir Sabantsev").reviews__author-pic
                .reviews__author-info
                  span.reviews__author-name Владимир Сабанцев
                  span.reviews__author-occ Преподаватель
              .reviews__content
                p.reviews__info Этот код выдержит любые испытания. Только пожалуйста, не загружайте сайт на слишком старых браузерах
              .reviews__btns
                  button(type="button").btn.btn-edit Править
                  button(type="button").btn.btn-delete Удалить

            li.reviews__item
              .reviews__item-top
                .reviews__author-img
                  img(src="../images/content/Vladimir.jpg" alt="Vladimir Sabantsev").reviews__author-pic
                .reviews__author-info
                  span.reviews__author-name Владимир Сабанцев
                  span.reviews__author-occ Преподаватель
              .reviews__content
                p.reviews__info Этот код выдержит любые испытания. Только пожалуйста, не загружайте сайт на слишком старых браузерах
              .reviews__btns
                  button(type="button").btn.btn-edit Править
                  button(type="button").btn.btn-delete Удалить
            li.reviews__item
              .reviews__item-top
                .reviews__author-img
                  img(src="../images/content/Vladimir.jpg" alt="Vladimir Sabantsev").reviews__author-pic
                .reviews__author-info
                  span.reviews__author-name Владимир Сабанцев
                  span.reviews__author-occ Преподаватель
              .reviews__content
                p.reviews__info Этот код выдержит любые испытания. Только пожалуйста, не загружайте сайт на слишком старых браузерах
              .reviews__btns
                  button(type="button").btn.btn-edit Править
                  button(type="button").btn.btn-delete Удалить
            li.reviews__item
              .reviews__item-top
                .reviews__author-img
                  img(src="../images/content/Vladimir.jpg" alt="Vladimir Sabantsev").reviews__author-pic
                .reviews__author-info
                  span.reviews__author-name Владимир Сабанцев
                  span.reviews__author-occ Преподаватель
              .reviews__content
                p.reviews__info Этот код выдержит любые испытания. Только пожалуйста, не загружайте сайт на слишком старых браузерах
              .reviews__btns
                  button(type="button").btn.btn-edit Править
                  button(type="button").btn.btn-delete Удалить


        


              
                  






    









</template>


<style lang="postcss">
@import url('https://fonts.googleapis.com/css?family=Open+Sans:300,400,600,700,800');
@import "normalize.css";
@import "../styles/mixins.pcss";
@import "../styles/layout/base.pcss";
@import "../styles/admin/login.pcss";
@import "../styles/admin/header.pcss";
@import "../styles/admin/nav.pcss";
@import "../styles/admin/main-content.pcss";
@import "../styles/admin/about.pcss";
@import "../styles/admin/cards.pcss";
@import "../styles/admin/works.pcss";
@import "../styles/admin/reviews.pcss";
@import "../styles/admin/form.pcss";
</style>