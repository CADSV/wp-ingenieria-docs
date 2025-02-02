# Formulario de Ofertas
****
## Descripción
_Este documento explica la configuración y utilización del formulario de ofertas_

## Modo de Acceso al Formulario

1. En la página del administrador de Wordpress de su escuela, acceder a la sección de **Contacto** > **Formulario de Contacto**.
<p align="center"><img src="https://imgur.com/8jR7CaV.png"/></p> 

2. Seleccionar el formulario ya creado que aparece la lista de formularios. Este puede tener el nombre de `Ofertas` o `Ofertas - Caracas` (dependiendo de la escuela).


<p align="center"><img src="https://imgur.com/uPXfoQV.png"/></p> 

### Características del formulario

Este formulario consta de 4 pestañas:

<p align="center"><img src="https://imgur.com/wot34Cr.png"/></p>

-  **Formulario**: Consiste en un editor de texto en donde se colocan los shortcodes de divi para cada campo del formulario. Para más información sobre los shortcodes y las funcionalidades de este formulario, consultar la [documentación](https://contactform7.com/editing-form-template/).

- **Correo**: En esta pestaña, se hacen las configuraciones de envío de correo electrónico. los campos que se muestran son:
    1. **Para**: En este campo se coloca el correo electrónico a quien se enviará el correo.
    2. **De**: En este campo se coloca el correo electrónico desde el que se enviará el correo. Por default es el correo de wordpress de la facultad. no es necesario cambiarlo.
    3. **Asunto**: En este campo se coloca el asunto del correo.
    4. **Cabeceras Adicionales**: Puede insertar campos de encabezado de mensaje adicionales aquí, como Cc y Bcc . Debe haber un campo por línea. 
    5. **Cuerpo del Mensaje**: En este campo se coloca el cuerpo del mensaje que se enviará.
    6. **Adjuntos**: En este campo se colocan los archivos que se adjuntarán al correo.

    Al correo se le pueden agregar shortcodes para colocar los datos del formulario. Por ejemplo, si se coloca el shortcode `[nombre]` en el campo de correo, se colocará el valor del campo de nombre. Para más información sobre los shortcodes, consultar la [documentación](https://contactform7.com/setting-up-mail/).

- **Mensajes**: En esta pestaña se configuraran todos los mensajes que el formulario mostrará.Mensajes de éxito, de error, de confirmación, etc. Para más información sobre los mensajes, consultar la [documentación](https://contactform7.com/editing-messages/).

- **Ajustes Adicionales**: Puede incluir configuraciones adicionales para cada formulario de contacto agregando fragmentos de código en el formato específico en el panel de la pestaña Configuración adicional en la pantalla del editor de formularios de contacto. Casos como solo permitir el uso de formularios a los suscritos, modo demostración, código Javascript, etc. Para más información sobre los ajustes adicionales, consultar la [documentación](https://contactform7.com/additional-settings/).

## Configuración del formulario de Ofertas

### **Pestaña de Formulario**
En esta pestaña estan los shortcodes de divi para cada campo del formulario. Cabe destacar que este complemento de divi genera un formulario sin diseño alguno, es por ello que además de los shortcodes estan inscrustados etiquetas `HTML` con clases para poder usar el tema de formulario de la facultad.

<p align="center"><img src="https://imgur.com/8mTFGG9.png"/></p>

#### Los campos del formulario son:
 
- **Nombre de la Oferta**: Este campo es obligatorio.
- **Nombre de la Empresa**: Este campo es obligatorio.
- **Sitio Web**: Este campo es obligatorio.
- **Nombre del Autor de la Oferta**: Este campo es obligatorio.
- **Número de teléfono del Autor de la Oferta**: Este campo es obligatorio.
- **Correo electrónico del Autor de la Oferta**: Este campo es obligatorio.
- **Descripción de la Oferta**: Este campo es obligatorio.
- **Url de la Imagen Destacada de la Oferta**: Este campo es obligatorio.
- **Modalidad del Contrato**: Este campo es obligatorio.
- **Requisitos del Cargo**: Este campo es obligatorio.

### Pestaña de Correo

En esta vista se configuró los shortcodes anteriores en el cuerpo del mensaje. A continuación se muestra un ejemplo del mismo

```
De: [nombre] <[correo_electronico]>
Asunto: [post-title]

Nombre de la oferta:
[post-title]

Nombre de la empresa:
[nombre_de_la_empresa]

Sitio web:
[sitio_web]

Nombre del Contacto:
[nombre]

Numero de teléfono:
[numero_de_telefono]

Correo electrónico:
[correo_electronico]

Descripción del cargo:
[descripcion_del_cargo]

Imagen destacada:
<img src="[your-file]" style="border-style:solid" /> 

Modalidad del contrato:
[modalidad_de_contrato]

Requisitos del cargo:
[requisitos]





Luego de comprobar esta información y ponerse en contacto con la empresa en cuestión, si se desea publicar la oferta en la página web, deberá cargar la información del presente correo en el pod de ofertas.

-- 
Este mensaje se ha enviado desde un formulario de contacto en [_site_title] ([_site_url])
```

El correo al cual llegará la oferta es al encargado de las prácticas empresariales de cada escuela.

## Como colocar el formulario en una página

1. Copiar el shortcode `[contact-form-7 id="__ID_FORMULARIO__" title="__TITULO_FORMULARIO__"]` en la página donde desea colocar el formulario. Utilice un componente de código o de texto de los que provee DIVI. Para más información, consultar en la [documentación](https://www.elegantthemes.com/documentation/divi/code/) de DIVI.

**Pista**: El id del formulario y el titulo aparecen en la vista de configuración del formulario. y en la Lista de formularios de contacto.

<p align="center"><img src="https://imgur.com/pDYmyOR.png"/></p>
