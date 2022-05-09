# Spring JPA - Hibernate

|Annotation|Beschreibung|
|-|-|
|@Entity|Markiert eine Klasse als Ressource für die Datenbank|
|@Transient|Markiert ein Attribut, damit es nicht in die Datenbank eingebunden wird|
|@Id|Markiert ein Attribut als Id (Primary Key)|
|@Repository|Markiert ein Interface als Repository|
|@NoArgsConstructor|Wird verwendet, um einen Constructor ohne Argumente in einer Klasse zu erstellen (Wird für die Bean benötigt, da diese die Argumente nicht kennt)|
|@SequenceGenerator(name = "name", allocationSize = 1)|Generiert eine Sequenz für ein Attribut name gibt den Namen der Sequenz an. allocationSize ist die Anzahl, um die hochgezählt wird|
|@Repository|Legt ein Repository für die Datenbank an (Sollte JpaRepository<T,P> einbinden)|
|@GeneratedValue(strategy, generator)|Generiert einen Wert für das Attribut, die "strategy" gibt an, wie diese Attribut generiert werden soll. Zudem kann man einen "generator" übergeben, welcher den Namen einer Sequence als Parameter übernimmt|
|@OneToMany(mappedBy)|Gibt eine Referenz (Foreign key auf eine andere Tabelle an), "mappedBy" gibt den Namen der Tabelle an, auf welche referenziert werden soll|
|@ManyToMany||