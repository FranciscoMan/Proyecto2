# Proyecto2
Para el siguiente proyecto el proyecto se necesitara contar con android studio 3.0 o versiones más recientes

## Proposito
El desarrollo se basa en crear una aplicacion que funcione como una encuesta sobre cualquier tema
la cual luego de ser contestaba recopilará los resultados en un archivo txt y se enviará por correo.
Incluyendo la implementacion RadioButton, CheckBox y EditText

![Una imagen cualquiera](https://github.com/FranciscoMan/Proyecto2/blob/master/preview.png "Muestra")

## Archivo de diseño XML
~~~
<?xml version="1.0" encoding="utf-8"?>
<android.support.constraint.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <ScrollView
        android:layout_width="match_parent"
        android:layout_height="match_parent">

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:orientation="vertical">

            <ImageView
                android:id="@+id/imageView"
                android:layout_width="match_parent"
                android:layout_height="150dp"
                app:srcCompat="@drawable/logo"/>

            <TextView
                style="@style/CategoryStyle"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:background="#000000"
                android:text="@string/p1" />

            <RelativeLayout
                android:layout_width="wrap_content"
                android:layout_height="wrap_content">

                <RadioGroup
                    android:id="@+id/rdgGrupoP1"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_column="0"
                    android:layout_span="3"
                    android:checkedButton="@+id/rdbOne"
                    android:orientation="horizontal">
                    <RadioButton
                        android:id="@+id/rdbOne"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:text="Nada" />

                    <RadioButton
                        android:id="@+id/rdbTwo"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:text="Poco" />

                    <RadioButton
                        android:id="@+id/rdbThree"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:text="Un porron" />
                </RadioGroup>
            </RelativeLayout>

            <TextView
                style="@style/CategoryStyle"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:background="#000000"
                android:text="@string/p2" />

            <RelativeLayout
                android:layout_width="wrap_content"
                android:layout_height="wrap_content">

                <RadioGroup
                    android:id="@+id/rdgGrupoP2"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_column="0"
                    android:layout_span="3"
                    android:checkedButton="@+id/rdbOne"
                    android:orientation="horizontal">

                    <RadioButton
                        android:id="@+id/rdbOneP2"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:text="Si" />

                    <RadioButton
                        android:id="@+id/rdbTwoP2"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:text="No" />
                </RadioGroup>
            </RelativeLayout>

            <TextView
                style="@style/CategoryStyle"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:background="#000000"
                android:text="@string/p3" />

            <RelativeLayout
                android:layout_width="wrap_content"
                android:layout_height="wrap_content">

                <RadioGroup
                    android:id="@+id/rdgGrupoP3"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_column="0"
                    android:layout_span="3"
                    android:checkedButton="@+id/rdbOne"
                    android:orientation="horizontal">

                    <RadioButton
                        android:id="@+id/rdbOneP3"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:text="Si"
                        android:focusedByDefault="true"/>

                    <RadioButton
                        android:id="@+id/rdbTwoP3"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:text="No" />
                </RadioGroup>
            </RelativeLayout>

            <TextView
                style="@style/CategoryStyle"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:background="#000000"
                android:text="@string/p4" />

            <RelativeLayout
                android:layout_width="wrap_content"
                android:layout_height="wrap_content">

                <EditText
                    android:id="@+id/p4Text"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:ems="20"
                    android:inputType="textPersonName"
                    android:text="$$"
                    android:focusedByDefault="false"/>

            </RelativeLayout>

            <TextView
                style="@style/CategoryStyle"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:background="#000000"
                android:text="@string/p5" />

            <RelativeLayout
                android:layout_width="wrap_content"
                android:layout_height="wrap_content">

                <RadioGroup
                    android:id="@+id/rdgGrupoP5"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_column="0"
                    android:layout_span="3"
                    android:checkedButton="@+id/rdbOne"
                    android:orientation="horizontal">

                    <RadioButton
                        android:id="@+id/rdbOneP5"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:text="Si" />

                    <RadioButton
                        android:id="@+id/rdbTwoP5"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:text="No" />
                </RadioGroup>
            </RelativeLayout>

            <TextView
                style="@style/CategoryStyle"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:background="#000000"
                android:text="@string/p6" />

            <RelativeLayout
                android:layout_width="wrap_content"
                android:layout_height="wrap_content">

                <RadioGroup
                    android:id="@+id/rdgGrupoP6"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_column="0"
                    android:layout_span="3"
                    android:checkedButton="@+id/rdbOne"
                    android:orientation="horizontal">

                    <RadioButton
                        android:id="@+id/rdbOneP6"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:text="Poca" />

                    <RadioButton
                        android:id="@+id/rdbTwoP6"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:text="Indescriptible" />

                    <RadioButton
                        android:id="@+id/rdbThreeP6"
                        android:layout_width="wrap_content"
                        android:layout_height="wrap_content"
                        android:text="Un orgasmo tantrico" />
                </RadioGroup>
            </RelativeLayout>

            <TextView
                style="@style/CategoryStyle"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:background="#000000"
                android:text="@string/p7" />

            <RelativeLayout
                android:layout_width="wrap_content"
                android:layout_height="wrap_content">

                <EditText
                    android:id="@+id/p7Text"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:ems="20"
                    android:inputType="textPersonName"
                    android:text="..."
                    android:focusedByDefault="false"/>
            </RelativeLayout>

            <TextView
                style="@style/CategoryStyle"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:background="#000000"
                android:text="@string/p8" />

            <CheckBox
                android:id="@+id/ps4"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:text="Play Station 4" />

            <CheckBox
                android:id="@+id/xbox"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:text="Xbox One" />

            <CheckBox
                android:id="@+id/Pc"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:text="PC" />

            <TextView
                style="@style/CategoryStyle"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:background="#000000"
                android:text="Gracias por contestar!!" />

            <Button
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:onClick="enviar_Encuesta"
                android:text="Enviar Encuesta"
                android:textSize="20sp" />
        </LinearLayout>
    </ScrollView>

</android.support.constraint.ConstraintLayout>
~~~

## Archivo de ejecucion Java
~~~
import android.content.Intent;
import android.net.Uri;
import android.os.Environment;
import android.support.annotation.NonNull;
import android.support.v7.app.AlertDialog;
import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.CheckBox;
import android.widget.EditText;
import android.widget.RadioGroup;

import java.io.File;
import java.io.FileOutputStream;
import java.io.IOException;

public class MainActivity extends AppCompatActivity {
  //Declaracion de variables, una por radio group y un string al igual
    private RadioGroup p1;
    private RadioGroup p2;
    private RadioGroup p3;
    private RadioGroup p5;
    private RadioGroup p6;
    private String pR1="";
    private String pR2="";
    private String pR3="";
    private String pR5="";
    private String pR6="";

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        //declaramos los radioGroup
        p1 = (RadioGroup) findViewById(R.id.rdgGrupoP1);
        p2 = (RadioGroup) findViewById(R.id.rdgGrupoP2);
        p3 = (RadioGroup) findViewById(R.id.rdgGrupoP3);
        p5 = (RadioGroup) findViewById(R.id.rdgGrupoP5);
        p6 = (RadioGroup) findViewById(R.id.rdgGrupoP6);
        //grupo 1
        //agregamos el listener para cuando se seleccione uno de ellos se agregue la respuesta
        //al string correspondiente
        //Esto para cada redioGroup
        p1.setOnCheckedChangeListener(new RadioGroup.OnCheckedChangeListener(){

            @Override
            public void onCheckedChanged(RadioGroup group, int checkedId) {
                // TODO Auto-generated method stub
                if (checkedId == R.id.rdbOne){
                    pR1 ="Nada";
                }else if (checkedId == R.id.rdbTwo){
                    pR1 ="Poco";
                }else if (checkedId == R.id.rdbThree){
                    pR1 ="Un Porron";
                }
            }

        });
        //grupo 2
        p2.setOnCheckedChangeListener(new RadioGroup.OnCheckedChangeListener(){

            @Override
            public void onCheckedChanged(RadioGroup group, int checkedId) {
                // TODO Auto-generated method stub
                if (checkedId == R.id.rdbOneP2){
                    pR2 ="Si";
                }else if (checkedId == R.id.rdbTwoP2){
                    pR2 ="No";
                }
            }

        });
        //grupo 3
        p3.setOnCheckedChangeListener(new RadioGroup.OnCheckedChangeListener(){

            @Override
            public void onCheckedChanged(RadioGroup group, int checkedId) {
                // TODO Auto-generated method stub
                if (checkedId == R.id.rdbOneP3){
                    pR3 ="Si";
                }else if (checkedId == R.id.rdbTwoP3){
                    pR3 ="No";
                }
            }

        });

        //grupo 5
        //No es que nos hallamos saltado un grupo, sino que el numero del grupo es correspondiente a la pregunta
        p5.setOnCheckedChangeListener(new RadioGroup.OnCheckedChangeListener(){

            @Override
            public void onCheckedChanged(RadioGroup group, int checkedId) {
                // TODO Auto-generated method stub
                if (checkedId == R.id.rdbOneP5){
                    pR5 ="Si";
                }else if (checkedId == R.id.rdbTwoP5){
                    pR5 ="No";
                }
            }

        });

        //grupo 6
        p6.setOnCheckedChangeListener(new RadioGroup.OnCheckedChangeListener(){

            @Override
            public void onCheckedChanged(RadioGroup group, int checkedId) {
                // TODO Auto-generated method stub
                if (checkedId == R.id.rdbOneP6){
                    pR6 ="Poco";
                }else if (checkedId == R.id.rdbTwoP6){
                    pR6 ="Indescriptible";
                }else if (checkedId == R.id.rdbThreeP6){
                    pR6 ="Un orgasmo tantrico";
                }
            }

        });
    }


  //este metodo es el que se ejecuta al presionar el boton de ENVIAR
    void enviar_Encuesta(View v) throws IOException {
    //el string correo será lo que se escribirá en el archivo a enviar
        String correo ="Gracias por contestar! :)";
        //agregando espacios para orden
        correo=correo+"\n";
        //estas 3 variables corresponden a los 3 checkbox de la ultima pregunta
        CheckBox ps4 = findViewById(R.id.ps4);
        CheckBox xbox = findViewById(R.id.xbox);
        CheckBox Pc = findViewById(R.id.Pc);
        //de aqui en adelante se captura y agrega la respuesta de cada pregunta a la variable correo
        //P1
        //primero la pregunta
        correo = correo +getResources().getString(R.string.p1)+"\n";
        //luego la respuesta
        correo = correo +pR1+"\n";
        //P2
        correo = correo +getResources().getString(R.string.p2)+"\n";
        correo = correo +pR2+"\n";
        //P3
        correo = correo +getResources().getString(R.string.p3)+"\n";
        correo = correo +pR3+"\n";
        //P4
        correo = correo +getResources().getString(R.string.p4)+"\n";
        //aqui, tanto como en la pregunta 7 se utiliza un metodo auxiliar
        correo = correo +getP4()+"\n";
        //p5
        correo = correo +getResources().getString(R.string.p5)+"\n";
        correo = correo +pR5+"\n";
        //p6
        correo = correo +getResources().getString(R.string.p6)+"\n";
        correo = correo +pR6+"\n";
        //p7
        correo = correo +getResources().getString(R.string.p7)+"\n";
        //aqui como en la pregunta 4 se utiliza un metodo auxiliar
        correo = correo +getP7()+"\n";
        //p8
        correo = correo +getResources().getString(R.string.p8)+"\n";
        //aqui en la pregunta 8 como la respuesta es multiple
        //utilizamos varios if por si se seleccionaron más casillas
        if(ps4.isChecked()){
            correo = correo +"Play Station 4"+"\n";
        }
        if(xbox.isChecked()){
            correo = correo +"Xbox One"+"\n";
        }
        if(Pc.isChecked()){
            correo = correo +"Pc"+"\n";
        }
        
        //ahora procedemos a crear el archivo que será escrito en la memoria externa
        File internalStorageDir = getFilesDir();
        //nombramos el archivo como Encueesta.txt
        File enc = new File(Environment.getExternalStorageDirectory().getAbsolutePath(), "Encueesta.txt");


        // Creamos el flujo de salida para con él poder realizar la escritura
        FileOutputStream fos = new FileOutputStream(enc,false);
        // Escribimos en el archivo
        fos.write(correo.getBytes());
        // Cerramos el flujo de escritura
        fos.close();
        //aqi creamos un uri con el archivo creado para poder enviarlo por correo
        Uri path = Uri.fromFile(enc);
        //metodo auxiliar para enviar por correo la respuesta
        mail(path);

    }
    //este es el metodo del correo
    private void mail(Uri b){
        //creamos un intent para acceder a las aplicaciones de correo
        Intent intent = new Intent(Intent.ACTION_SEND);
        //Justo esta linea es para especificar que sólo aplicaciones que puedan manejar correo
        intent.setType("vnd.android.cursor.dir/email");
        //el Asunto se agrega
        intent.putExtra(Intent.EXTRA_SUBJECT, "Encuesta Ciberpunk 2077");
        //y aqui simplemente agregamos la uri con el archivo creado
        intent.putExtra(Intent.EXTRA_STREAM, b);
        //esto de aqui es para que en caso de que el intent sea exitoso en el grupo de aplicaciones
        //que nos regresa el sistema se vea el encabezado con "Send email..." lo cual es modificable al gusto
        //en caso de no se así mandaría un mensaje de alerta
        if (intent.resolveActivity(getPackageManager()) != null) {
            startActivity(Intent.createChooser(intent , "Send email..."));
        }else{
            //metodo auxiliar para mandar el mensaje de alerta
            alerta("No se ha podido acceder a las aplicaciones de calendario");
        }
    }
    
    //este metodo sirve para enviar un mensaje de alerta con lo que sea que contenga el parametro cadena
    public void alerta(String cadena) {
        AlertDialog.Builder dialogBuilder = new AlertDialog.Builder(this);
        dialogBuilder.setMessage(cadena);
        dialogBuilder.setCancelable(true).setTitle("Error");
        dialogBuilder.create().show();
    }
    
    //los siguientes dos metodos son para capturar el texto de los TextEdit de la pregunta 7 y 4
    @NonNull
    private String getP7(){
        EditText ed = findViewById(R.id.p7Text);
        return ed.getText().toString();
    }

    @NonNull
    private String getP4(){
        EditText ed = findViewById(R.id.p4Text);
        return ed.getText().toString();
    }




}

~~~


# Recurso de valores
***
## Colors.xml
~~~
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <color name="colorPrimary">#008577</color>
    <color name="colorPrimaryDark">#00574B</color>
    <color name="colorAccent">#D81B60</color>
</resources>
~~~
***
## Dimen.xml
~~~
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <dimen name="list_item_height">88dp</dimen>
    <!-- Default screen margins, per the Android Design guidelines. -->
    <dimen name="activity_horizontal_margin">16dp</dimen>
    <dimen name="activity_vertical_margin">16dp</dimen>

</resources>
~~~
***
## Strings.xml
~~~
<resources>
    <string name="app_name">Feedback</string>
    <string name="p1">¿Qué tan interesado se siente en el nuevo Ciberpunk 2077? </string>
    <string name="p2">¿Tiene conocimiento de su fecha de salida?</string>
    <string name="p3">¿Planea comprar el videojuego?</string>
    <string name="p4">¿Cuándo gasta al año en videojuegos?</string>
    <string name="p5">¿Asistió a la conferencia E3 de este año?</string>
    <string name="p6">¿Qué tanta es su emoción por el nuevo Ciberpunk 2077?</string>
    <string name="p7">Personalmente, ¿qué espera del título?</string>
    <string name="p8">¿Qué Plataformas usted tiene?</string>
</resources>
~~~
***
## Styles.xml
~~~
<resources>

    <!-- Base application theme. -->
    <style name="AppTheme" parent="Theme.AppCompat.Light.DarkActionBar">
        <!-- Customize your theme here. -->
        <item name="colorPrimary">@color/colorPrimary</item>
        <item name="colorPrimaryDark">@color/colorPrimaryDark</item>
        <item name="colorAccent">@color/colorAccent</item>
    </style>

    <style name="MyTheme" parent="Base.Theme.AppCompat.Light.DarkActionBar">
        <!-- Customize your theme here. -->
        <item name="colorPrimary">#009688</item>
        <item name="colorPrimaryDark">#00796B</item>
        <item name="colorAccent">@color/colorAccent</item>
    </style>

    <style name="CategoryStyle">
        <item name="android:layout_width">match_parent</item>
        <item name="android:layout_height">@dimen/list_item_height</item>
        <item name="android:gravity">center_vertical</item>
        <item name="android:padding">16dp</item>
        <item name="android:textColor">@android:color/white</item>
        <item name="android:textStyle">bold</item>
        <item name="android:textAppearance">?android:textAppearanceMedium</item>
    </style>
</resources>
~~~


