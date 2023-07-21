# Documento que detalla el proceso

Para el estilo general de la página html se inició haciendo un reset básico de todos los elementos (*), esto establece márgenes y rellenos en 0 para todos los elementos y el box-sizing se establece en "border-box". Posteriormente se añadieron estilos básicos a todos los elementos y al body de la aplicación, tipo de fuente (font-family), altura mínima del body (min-height) se establecio en el 100% del alto de la ventana (vh) y el body se configuró como un contenedor flexible (display: flex) con dirección de columna (flex-direction: column).

# Estilos para el encabezado (header):
El encabezado fue establecido como un contenedor flexible (display: flex) con alineación vertical centrada (align-items: center) y distribución horizontal equitativa (justify-content: space-between). Esto para colocar a los elementos hijos dentro del encabezado en la misma línea y separarlos con el espacio disponible.

# Estilos para el menú de navegación (nav):
El menú de navegación fue establecido como un contenedor flexible (display: flex) con distribución horizontal equitativa (justify-content: space-between) para separar los enlaces de navegación.

# Estilos para el contenido principal y la barra lateral (main y aside):
El contenido principal (main) y la barra lateral (aside) se establecieron como contenedores flexibles (display: flex). El contenido principal utiliza flex-wrap: wrap para permitir que los elementos se envuelvan cuando no haya suficiente espacio en una sola línea y la propiedad justify-content: space-between se aplicó para distribuir los elementos del contenido principal y la barra lateral equitativamente en el espacio disponible.

Dentro del contenido principal (main), cada sección tiene un crecimiento flexible (flex: 1) para que ocupen el espacio disponible, pero con un ancho mínimo de 300 píxeles (min-width: 300px).

La barra lateral (aside) tiene un ancho mínimo de 200 píxeles (min-width: 200px) y un relleno de 10 píxeles.

# Estilos para el pie de página (footer):
El pie de página se estableció como un contenedor flexible (display: flex) con alineación vertical centrada (align-items: center) y distribución horizontal equitativa (justify-content: space-around) para separar los elementos del pie de página. 

# Media queries para diseño responsive:
Se definido una media queries para adaptar el diseño cuando el ancho de la pantalla es igual o menor a 768 píxeles, esto para aplicar las siguientes modificaciones para un diseño más adecuado para dispositivos móviles:
*	El contenido principal y la barra lateral cambian a una disposición de columna (flex-direction: column) para una visualización más vertical en dispositivos pequeños.
* La barra lateral (aside) ocupa todo el ancho disponible (min-width: 100%) para llenar el espacio disponible en pantallas estrechas.
*	El encabezado (header) también cambia a una disposición de columna y el texto se centrará (text-align: center).
