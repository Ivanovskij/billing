[![Build Status](https://travis-ci.org/we-are-comrades/billing.svg?branch=master)](https://travis-ci.org/we-are-comrades/billing)  [![Codacy Badge](https://api.codacy.com/project/badge/Grade/e4262d0680044f208141fdced3d38f59)](https://www.codacy.com/project/vrnsky/billing/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=we-are-comrades/billing&amp;utm_campaign=Badge_Grade_Dashboard) [![codecov](https://codecov.io/gh/we-are-comrades/billing/branch/master/graph/badge.svg)](https://codecov.io/gh/we-are-comrades/billing)

# Биллинговая система

Кратко разберем, что же такое биллинговая система, какие ее задачи и основные понятия.

> Биллинговая система - комплекс, осуществляющий учет объема потребляемых абонентами услуг, расчет и списание денежных средств в соответствии с тарифами компании.
> 
> **Денис Шергин, Java Developer**

Мы попробуем сделать упрощенную версию биллинговой системы, оперирующую транзакциями, основаная задача которых перевод денежных средств с одного счета на другой. 

Транзакция состоит из [операций](https://ru.wikipedia.org/wiki/%D0%94%D0%B5%D0%B1%D0%B5%D1%82_%D0%B8_%D0%BA%D1%80%D0%B5%D0%B4%D0%B8%D1%82): дебета, кредита.

![Alt text](https://pp.userapi.com/c830308/v830308518/5050c/2PaCHT_cQ8Y.jpg)

Какие задачи решает биллинговая система?

* Осуществление обработки операций.
* Контроль денежных средств на счетах пользователей.
* Предоставление статистики по операциям.
* Обеспечение надежности и защищенности обработки операций.

Представим ситуацию, что текущая биллинговая система не соответствует требованиям высшего руководства и нуждается в высоких затратах на поддержку. Множество платных решений, которые присутствуют на рынке, не удовлетворяют критерям, постваленным компанией.

По этой причине вам необходимо реализовать новую биллинговую систему, которая будет способна обработать порядка **1000 транзакций** в секунду и уменьшит нагрузку на веб-сервер и базу данных. При в системе должна быть возможность предоставить статистику и информацию по всем операциям в доступном для бухгалтеров и других сотрудников формате.

![Alt text](https://pp.userapi.com/c830708/v830708901/4cc6a/pl-GoUvVfII.jpg)

Разрабтаываемая биллинговая система должна состоять из следующих частей: 
* модуль обработки транзакций,
* модуль работы с аккаунтами - счетами пользователей.

Впереди вас ждут следующие этапы:
* Шаг #1. Подготовка;
* Шаг #2. Менеджер счетов;
* Шаг #3. Обработка транзакций.

> **Warning**: Все перечисленные шаги находятся во вкладке **Issues**!

## Стек технологий

Вам необходимо воспользоваться следующим стеком технологий в данном проекте:

* Maven
* Spring 
* Tomcat
* Slf4j
* JUnit
* Mockito
* PostgresSQL
