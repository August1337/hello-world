# hello-world
public class Uppgift6 extends Application {

    public static void main(String[] args) {
        launch(args);
    }

    @Override
    public void start(Stage primaryStage) {

        Label text = new Label("Ange tid:");
        Font moret = new Font("Moret",14);
        text.setFont(moret);


        TextField timme = new TextField();
        timme.setPrefSize(40,10);
        Label h = new Label("h");
        h.setFont(moret);

        TextField minut = new TextField();
        minut.setPrefSize(40,10);
        Label m = new Label("m");
        m.setFont(moret);

        TextField sekund = new TextField();
        sekund.setPrefSize(40,10);
        Label s = new Label("s");
        s.setFont(moret);

        HBox inmat = new HBox();
        inmat.setPadding(new Insets(10));
        inmat.setSpacing(5);
        inmat.getChildren().addAll(text,timme,h,minut,m,sekund,s);

        Scene scene = new Scene(inmat,300,300);
        primaryStage.setTitle("Beräkna tid");
        primaryStage.setScene(scene);
        primaryStage.show();



    }
}
