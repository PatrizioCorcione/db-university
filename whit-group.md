# Query whit group by

## Contare quanti iscritti ci sono stati ogni anno

- SELECT COUNT(`id`)
- FROM `students`
- GROUP BY YEAR(`enrolment_date`);

## Contare gli insegnanti che hanno l'ufficio nello stesso edificio

- SELECT COUNT(`id`)
- FROM `teachers`
- GROUP BY `office_address`;

## Calcolare la media dei voti di ogni appello d'esame

- SELECT AVG (`vote`)
- FROM `exam_student`
- GROUP BY `exam_id`

## Contare quanti corsi di laurea ci sono per ogni dipartimento

- SELECT COUNT(`id`)
- FROM `degrees`
- GROUP BY `department_id`;
