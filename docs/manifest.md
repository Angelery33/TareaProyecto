# El archivo AndroidManifest.xml

El **AndroidManifest.xml** es el archivo central de cualquier aplicación Android que contiene información obre ella.
Esta informacion es usada por *Android build tools* ,El sistema en sí mismo y google play.

Este archivo contiene informacion sobre :
- Los diferentes **componentes de la aplicación y sus propiedades**.
- Los **permisos de la aplicación**.


## Funciones principales

1. **Define componentes** (actividades, servicios, receptores).  
2. **Especifica permisos** que requiere la aplicación.  
3. **Declara el punto de entrada** (actividad principal).  

## Ejemplo de manifest

```
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    package="com.example.myapp">

    <application
        android:label="@string/app_name"
        android:icon="@mipmap/ic_launcher"
        android:theme="@style/Theme.MyApp">

        <activity android:name=".MainActivity">
            <intent-filter>
                <action android:name="android.intent.action.MAIN"/>
                <category android:name="android.intent.category.LAUNCHER"/>
            </intent-filter>
        </activity>

    </application>
</manifest>

