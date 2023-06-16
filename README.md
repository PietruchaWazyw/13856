# 13856
Wymagania wstępne
Aby uruchomić testy opisane w tym przewodniku, będziesz potrzebować:

* Zainstalowanego Java Development Kit (JDK) w wersji 8 lub nowszej.
* Środowiska uruchomieniowego Apache Maven lub Gradle.

Testowanie ładowania kontekstu aplikacji
1. Otwórz plik src/test/java/com/example/testingweb/TestingWebApplicationTests.java.
2. W pliku znajduje się klasa TestingWebApplicationTests, która jest klasyfikowana jako test jednostkowy przy użyciu adnotacji @RunWith(SpringRunner.class).
3. Klasa ta zawiera metodę testową contextLoads(), która sprawdza, czy kontekst aplikacji poprawnie się ładuje. Możesz to zrobić, używając adnotacji @SpringBootTest, która uruchamia pełny kontekst aplikacji Spring podczas testu.
4. Uruchom test przy użyciu narzędzia do budowania projektu. Na przykład, jeśli używasz Maven, wykonaj polecenie:
mvn test
Jeśli używasz Gradle, wykonaj polecenie:
gradle test
5. Test powinien zakończyć się pomyślnie, a w konsoli powinno pojawić się powiadomienie o poprawnym ładowaniu kontekstu aplikacji.

Testowanie warstwy webowej przy użyciu Spring MockMvc
1. Otwórz plik src/test/java/com/example/testingweb/HomeControllerTest.java.
2. W pliku znajduje się klasa HomeControllerTest, która zawiera testy jednostkowe dla kontrolera HomeController.
3. Klasa ta używa narzędzia Spring MockMvc, które pozwala na symulowanie żądań HTTP i testowanie warstwy webowej bez potrzeby uruchamiania aplikacji na prawdziwym serwerze.
4. Testy w tej klasie pokazują, jak przetestować interakcje między kontrolerem a warstwą webową.
5. Uruchom testy, używając narzędzia do budowania projektu, tak jak opisano wcześniej.
6. Testy powinny zakończyć się pomyślnie, a wyniki zostaną wyświetlone w konsoli.
