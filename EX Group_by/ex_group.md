1. Contare quanti iscritti ci sono stati ogni anno
-SELECT YEAR(enrolment_date) AS anno, COUNT(*) AS numero_iscritti FROM students GROUP BY YEAR(enrolment_date) ORDER BY anno;

2. Contare gli insegnanti che hanno l'ufficio nello stesso edificio
-SELECT office_address, COUNT(*) as numero_insegnanti FROM teachers GROUP BY office_address;


3. Calcolare la media dei voti di ogni appello d'esame
-SELECT exam_id, AVG(vote) as media_voti FROM exam_student GROUP BY exam_id;

4. Contare quanti corsi di laurea ci sono per ogni dipartimento