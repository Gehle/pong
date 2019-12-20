# Pongspiel:

Programmieren II / Software Engineering Projekt



Mitglieder: Matthieu Doerler, Jules Beyel, Emilie Gehl


### Inhaltsverzeichnis

1. [Einleitung](#einleitung)
    + [Ziele](#ziele)
    + [Randbedingungen](#randbedingungen)
1. [Build-Anleitung](#build-anleitung)
1. [Bedienungsanleitung](#bedienungsanleitung)
1. [Userstories](#userstories)
1. [Releaseplan](#releaseplan)
1. [Dokumentation Sprint 1](#dokumentation-sprint-1)
    + [Taskliste für die Umsetzung der Userstories](#taskliste-für-die-umsetzung-der-userstories)
    + [Dokumentation wichtiger Code Snippets](#dokumentation-wichtiger-code-snippets)
    + [Testfaelle in Bezug auf Akzeptanzkritierium](#testfaelle-in-bezug-auf-akzeptanzkritierium)
    
1. [Dokumentation Sprint 2](#dokumentation-sprint-2)
    + [Taskliste für die Umsetzung der Userstories](#taskliste-für-die-umsetzung-der-userstories)
    + [Dokumentation wichtiger Code Snippets](#dokumentation-wichtiger-code-snippets)
    + [Testfaelle in Bezug auf Akzeptanzkritierium](#testfaelle-in-bezug-auf-akzeptanzkritierium)
1. [Ergebnisse nach Umsetzung der Userstories](#ergebnisse-nach-umsetzung-der-userstories)
1. [Klassendiagramm](#klassendiagramm)

# Software Engineering

## 1. Einleitung
Willkommen zu unserem Projekt. Wir haben ein Spiel für Menschen im Alter von 5 bis 99 Jahren entwickelt. Es kann einzeln abgespielt werden und es ist keine Internetverbindung erforderlich. Es ist eine tolle Möglichkeit, die Zeit zu verbringen und gleichzeitig Spaß zu haben.
### Ziele
Das Ziel ist es die erlernten Fähigkeiten und Kompetenzen im Bereich Programmieren und Software Engineering innerhalb eines einzigen Projektes in Verbindung zu bringen. Hierfür wollen wir das Spiel Pong programmieren. Auf einer graphischen Oberfläche soll unser Hauptprogramm (Das Spiel) originalgetreu dargestellt werden und unser Spiel darauf gespielt werden. Wir planen für dieses Projekt 2 Sprints.

### Randbedingungen
- Die Programmierung der Anwendung soll in JAVA erfolgen.
- Die Klassen des Programms sollen über die entsprechenden Unit-Tests verfügen.
- Das Projekt soll auf GitHub veröffentlich werden.
- Die Buildautomatisierung soll mit MAVEN erfolgen.
- Das Programm soll mittels einer dafür erstellten JAR-Datei und dem Befehl java-jar xxxxx.jar ausgeführt werden können.

## 2. Build-Anleitung

Git clone:  https://github.com/Gehle/pong
In Git program: 
1. Speichern Sie Ihre src Datei von Ihre Git Projekt auf Ihre Rechner.
2. Löschen Sie Ihre src Datei von Ihre Git Projekt.
3. Fügen Sie die pom.xml Datei mit die geeignete Initialiesierung in das Git Projekt.
4. Fügen Sie die src Ordner von einen Maven Projekt in das Git Projekt.
5. Klicken Sie auf den rechten Maus Taste in " pong": ->Configure ->Convert to Maven.
6. Fügen Sie Ihr eigenes Package in das Ordner src/main/java.
7. Klicken Sie auf den rechten Maus Taste in " pong": ->Run as ->Maven clean.
8. Klicken Sie auf den rechten Maus Taste in "pong": ->Run as ->Maven install.
9. Prüfen Sie in das Ordner "target" ob Sie eine Datei .jar haben.

## 3. Bedienungsanleitung

Nach dem Start unserer App entdecken Sie die Startseite. Nachdem Sie sich über die Spielregeln informiert haben oder nicht, klicken Sie auf "Start" und das Spiel beginnt. Der Ball darf nicht fallen, also bewegen Sie das Rechteck mit der Maus, um den Ball zu prallen. Ihr Ergebnis wird am Ende des Spiels angezeigt. Das ist, wie oft du es geschafft hast, den Ball zurückzuschicken. Viel Erfolg beim spielen !

## 4. Userstories

| **Userstory Nr.** |   **Userstories / Akzeptanzkriterien**  | **Storypoints**  |  **Priorität** |
|:-:|-----|:-:|:-:|
| 1 | Als Benutzer möchte ich verschiedene Schwierigkeitsgrade <br/>AK: Die Geschwindigkeit der Kugel beschleunigt sich. | 8 | 2 |
| 2 | Als Benutzer möchte ich das Spiel neustarten und verlassen können.<br/>AK: Neustart und Exit durch Buttons. | 2 | 2 |
| 3 | Als Benutzer möchte ich Hintergrundmusik mit einstellbarer Lautstärke.<br/>AK: SLider für die Musikstärke und Buttons für on/off. | 5 | 3 |
| 4 | Als Benutzer möchte ich meinen Punktestand sobald das Spiel fertig ist wissen.<br/>AK: Das Punktestand ist während Spiel gezeigt. | 5 | 2 |
| 5 | Als Benutzer möchte ich ohne Internetverbindung spielen.<br/> AK: Das Spiel soll offline gespielt werden können. | 5 | 2 |
| 6 | Als Programmierer möchte ich das Programm einfach nachvollziehen können um es nachbauen, warten und neue Features einfügen zu können.<br/>AK: Kommentare im Code. Logische Struktur (Klassen, Methoden, Variablen). | 3 | 1 |
| 7 | Als Benutzer möchte ich, dass das Spiel an meinen Computer angepasst ist.<br/>AK: Das Spiel ist für alle Bildschirmgrößen geeignet. | 3 | 1 |
| 8 | Als Benutzer möchte ich die Spielregeln kennenlernen.<br/> AK: Neue Fenster mit Spielregeln mit ein Button erreichbar. | 3 | 2 |

Legende : AK = Akzeptanzkriterium

## 5. Releaseplan
|  Release 1 | Release 2  |
|:-:|:-:|
|  US 1 | US 3  |
|  US 2 | US 4  |
|  US 5 | US 6  |
|  US 8 | US 7  |

Legende : US = Userstory

## 6. Dokumentation Sprint 1
###  Taskliste für die Umsetzung der Userstories
| Tasknummer | Tasks | Userstory | Geschätzter Aufwand |
|:-:|-----|:-:|:-:|
| 1 | Grafisches Layout erstellen | 1 | 3 Stunden |
| 2 | 4 Button für das Starten, Exit, Credits, und Spielregeln | 2 | 2 Stunden |
| 3 | 2 Fenster für Spielregeln und Credits | 8 | 2 Stunden |
| 4 | Neuer Klasse VueController | 1 | 1,5 Stunden |
| 5 | Das Ball und das Rechteck erstellen und platzieren | 1 | 1,5 Stunden |
| 6 | Ballgeschwindigkeit und -beuschleunigung erzeugen | 1 | 1,5 Stunden |
| 7 | Rückprall dem Ball berücksichtigen | 1 | 2 Stunden |
| 8 | Inbetriebnahme aller setOnAction (Mouse, Taste) | 1 | 1,5 Stunden |

### Dokumentation wichtiger Code Snippets

**Code um eine neue Fenster anzuzeigen**

            Pane layout = new Pane();
			FXMLLoader loader = new FXMLLoader();

			loader.setLocation(Main.class.getResource("Vue2.fxml"));
			layout = (Pane) loader.load();
			Scene scene = new Scene(layout);

			primaryStage.setScene(scene);
			primaryStage.show();
           
**Erstellung der Ball und Rechteck**

            Circle ball = new Circle(psx / 2, psy / 2, rball);
			ball.setFill(Color.WHITE);

			Rectangle joueur = new Rectangle((psx - lrect) / 2, rectY, lrect, hrect);																	
			joueur.setFill(Color.WHITE);
           

**Beschleunigung der Ball in einen Loop**

				loop = new Timeline(new KeyFrame(Duration.millis(5), new EventHandler<ActionEvent>() {
				public void handle(ActionEvent arg) {
					
					// deplacement:
					ball.setCenterX(ball.getCenterX() + ballSpeedX);
					ball.setCenterY(ball.getCenterY() - ballSpeedY);

					// haut
					if (ball.getCenterY() <= (rball / 2)) {
						ballSpeedY = -dy;
					}

					// bas
					if (ball.getCenterY() >= rectY) {
						if (ball.getCenterX() >= joueur.getX() && ball.getCenterX() <= joueur.getX() + lrect) {
							dx += 0.25;
							dy += 0.25;
							ballSpeedY = dy;
							score += 1;
						}
					}

					// gauche
					if (ball.getCenterX() <= (rball / 2)) {
						ballSpeedX = dx;
					}

					// droit
					if (ball.getCenterX() >= (psx - (rball / 2))) {
						ballSpeedX = -dx;
					}

					// collision bas
					if (ball.getCenterY() >= (psy - (rball / 2))) {
						text.setVisible(true);
						message.setVisible(true);
						loop.stop();
						/*ballSpeedX = 0;
						ballSpeedY = 0;
						ball.setCenterX(25);
						ball.setCenterY(25); 
						ball.setFill(Color.BLACK);
						ball.toBack();*/
						
						scene.setOnKeyPressed(new EventHandler<KeyEvent>() { // detecte si on a appui� sur une touche
							public void handle(KeyEvent event) {
								if (event.getCode() == KeyCode.ESCAPE) {
									Main.mainScene();
								}
								event.consume();
							}});
					}
					primaryStage.setTitle("Pong || Score: " + score);}}));
			loop.setCycleCount(Timeline.INDEFINITE);
			loop.play();
         



### Testfälle in Bezug auf Akzeptanzkriterium
| Testfall | Aus US/AK | Vorbedingung | Ablauf | Resultat |
|:-:|:-:|-----|-----|-----|
| 1 | 1 | Das Spiel wurde gestartet | Den Ball wurde mehrmals geprallt mit dem Rechteck | Der Ball beschleunigt sich |
| 2 | 2 | Das Spiel wurde gestartet | Klicken auf Exit und ESC am Ende des Spiels | Das Spiel wurde beendet und neugestartet |
| 3 | 5 | Internetverbindung ausfallen und dem Spiel starten | der Rechner steht in Flugzeugmodus | Das Spiel läuft gut |
| 4 | 8 | Das Spiel wurde gestartet | Klicken auf Knopf "Spielregeln" | Das Spielregelnfenster erscheint |

## 7. Dokumentation Sprint 2
###  Taskliste für die Umsetzung der Userstories
| Tasknummer | Tasks | Userstory | Geschätzter Aufwand |
|:-:|-----|:-:|:-:|
| 1 | 3 Button und ein Slider für Musiksteuerung | 3 | 1,5 Stunden |
| 2 | Fenstergrossebestimmung | 7 | 30 Minuten |
| 3 | Punktesumme und -anzeige | 4 | 30 Minuten |
| 4 | Anschliessende Botschaft, wenn das Spiel beendet ist | 4 | 30 Minuten |
| 5 | Klassendiagramm auf Eclipse erstellen | 6 | 20 Minuten |
| 6 | Dokumentation in Markdown Format in der README Datei schreiben (Projektbeschreiben) | 6 | 4 Stunden |
| 7 | Dokumentation in Markdown Format in der README Datei schreiben (Sprint 1) | 6 | 3 Stunden |
| 8 | Dokumentation in Markdown Format in der README Datei schreiben (Sprint 2) | 6 | 3 Stunden |
| 9 | Kommentare in Programm hinzufügen | 6 | 30 Minuten |
| 10 | Testklasse schreiben (JUnit) | 6 | 1,5 Stunden |

### Dokumentation wichtiger Code Snippets

**Fenstergrossebestimmung (der Benutzer kann es nicht ändern)**

			primaryStage.setResizable(false);
			primaryStage.setScene(scene);
			primaryStage.setTitle("Pong");
			primaryStage.show();
            

**Die Musik in den Ordner holen**

		File file = new File(getClass().getResource("arcade.mp3").toString());
		String path = file.toURI().toString();
		
		media = new Media(getClass().getResource("arcade.mp3").toString());
		mediaplayer = new MediaPlayer(media);
		System.out.println(media.toString());
        

**Musiksteuerung**

	@FXML
	public void playSound(ActionEvent event) {
		mediaplayer.play();
	}

	@FXML
	public void volume(ActionEvent event) {
		mediaplayer.setVolume(sldQuertety.getValue());
	}

	@FXML
	public void pause(ActionEvent event) {
		mediaplayer.pause();
	}

	@FXML
	public void change(ActionEvent event) {
		mediaplayer.setVolume(sldQuertety.getValue());
	}
    

### Testfälle in Bezug auf Akzeptanzkriterium
| Testfall | Aus US/AK | Vorbedingung | Ablauf | Resultat |
|:-:|:-:|-----|-----|-----|
| 1 | 3 | Das Spiel wurde gestartet | Auf den Knopf für die Musiksteuerung drücken | Die Musik wurde gestartet und gestoppt |
| 2 | 4 | Das Spiel wurde gestartet | Der Ball mehrmalls prellen | Der Punktestand erhöht sich |


## 8. Ergebnisse nach Umsetzung der Userstories

![](src/main/resources/images/Startseite.PNG)

![](src/main/resources/images/Spielregeln.PNG)

![](src/main/resources/images/Spiel.PNG)

## 9. Klassendiagramm

![](src/main/resources/images/Klassendiagramm.jpeg)
