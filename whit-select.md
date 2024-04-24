# Query whit SELECT

## Seleziona tutti gli studenti nati nel 1990

- SELECT \*
- FROM `students`
- WHERE YEAR(`date_of_birth`) = 1990

## Seleziona tutti i corsi che valgono più di 10 crediti

- SELECT \*
- FROM `courses`
- WHERE `cfu` > 10

## Seleziona tutti gli studenti con più di 30 anni

- SELECT \*
- FROM `students`
- WHERE TIMESTAMPDIFF(YEAR,`date_of_birth`,CURDATE())> 30B

## Seleziona tutti i corsi del primo semestre del primo anno di qualsiasi corso di laruea

- SELECT \*
- FROM `courses`
- WHERE `period` = 'I semestre'
- AND `year` = 1

## Seleziona tutti gli appelli di esame che avvengono ne pomeriggio (dopo le 14) del 2020-06-20

- SELECT \*
- FROM `exams`
- WHERE `date` = '2020-06-20'
- AND HOUR(`hour`) >= 14

## Seleziona tutti i corsi di lauerea magistrale

- SELECT \*
- FROM `degrees`
- WHERE `level` = 'magistrale'

## Da quanti dipartimenti è composta l'università

- SELECT COUNT(\*)
- FROM `departments`;

## Quanti sono gli insegnanti che non hanno il numero di telefono

- SELECT COUNT(\*)
- FROM `teachers`
- WHERE `phone` IS NULL
