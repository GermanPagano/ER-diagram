
<h1 align="center">
  <br>
  <a href="https://www.linkedin.com/in/gerhpagano/"><img src="https://www.ceteris.ag/fileadmin/user_upload/Dateien_Ceteris/Bilder/Illustrationen/Ceteris_Technologien_RGB_Azure_SQL_Database.png" style='max-height: 200px;'>
</a>
  <br>
  ER diagram for a university midterm exam
  <br>
</h1>

![parcial-PAGANO-SERGIO-GERMAN](https://user-images.githubusercontent.com/80891761/235391922-5d09028e-902c-4ff9-b746-c97e94b7ed86.png)



## Explanation of the diagram


<p><strong>Película:</strong> The movie table meets the requested information requirements in the prompt and I added a PK (PELICULA_ID). It will also have a FK (DIRECTOR_ID) because its cardinality with the Director table is N:1.</p>

<p><strong>Género:</strong> I created the genre table to be able to sort the different types of genres by their ID number (e.g. id: 1= name: Horror, id: 2= name: Action, etc.).</p>

<p><strong>Pelicula_X_Genero:</strong> As the cardinality between Película and Género is N:N, a new table will be generated composed of the PKs of both tables. This way, I believe it would be a simple way to relate the ID of the movie with the genre it belongs to.</p>

<p><strong>Actor:</strong> The Actor table meets the requirements requested in the prompt, and I also added a PK (ACTOR_ID). As it has a cardinality of N:N with respect to the movie, it will generate a new table.</p>

<p><strong>Pelicula_X_Actor:</strong> This table will match the PKs of Película and Actor, and will also have an additional attribute called Rol, where it will describe if the role of the actor mentioned by their ID is Protagonist, Extra, Antagonist, etc.</p>

<p><strong>Director:</strong> The Director table has a cardinality of N:1 with respect to Película. This table also has a PK (DIRECTOR_ID), which will be a numeric primary key and a foreign key in the movie table, specifying which director ID made the movie.</p>



