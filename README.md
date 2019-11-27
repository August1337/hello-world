# hello-world

public class Uppgift1 extends Application {

    public static void main(String[] args) {
        launch(args);
    }

    @Override
    public void start(Stage primaryStage) {

        Group layout = new Group();

        Circle liten = new Circle(250,100,50);
        liten.setFill(Color.WHITE);
        liten.setStroke(Color.WHITE);

        Circle mellan = new Circle(250,200,70);
        mellan.setFill(Color.WHITE);
        mellan.setStroke(Color.WHITE);

        Circle stor = new Circle(250,325,100);
        stor.setFill(Color.WHITE);
        stor.setStroke(Color.WHITE);

        Circle sol = new Circle(457,25,50);
        sol.setFill(Color.YELLOW);

        Circle knapp1 = new Circle(250,150,5);
        knapp1.setFill(Color.BLACK);
        knapp1.setStroke(Color.BLACK);

        Circle knapp2 = new Circle(250,170,5);
        knapp2.setFill(Color.BLACK);
        knapp2.setStroke(Color.BLACK);

        Circle knapp3 = new Circle(250,190,5);
        knapp3.setFill(Color.BLACK);
        knapp3.setStroke(Color.BLACK);

        Rectangle mun = new Rectangle(230,110,40,1);
        mun.setFill(Color.BLACK);
        mun.setRotate(24);;

        Circle eye1 = new Circle(230,80,10);
        eye1.setFill(Color.BLACK);

        Circle eye2 = new Circle(270,80,10);
        eye2.setFill(Color.BLACK);


        Rectangle rekt = new Rectangle(500,400);
        rekt.setFill(Color.MIDNIGHTBLUE);

        layout.getChildren().addAll(rekt,liten,mellan,stor,sol,knapp1,knapp2,knapp3,mun,eye1,eye2);

        Scene scene = new Scene(layout,500,500);
        primaryStage.setScene(scene);
        primaryStage.setTitle("Snowman");
        primaryStage.show();
    }
}
