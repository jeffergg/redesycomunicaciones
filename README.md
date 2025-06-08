from pptx import Presentation
from pptx.util import Inches, Pt

# Crear una nueva presentación
prs = Presentation()

def add_slide(title, content):
    slide_layout = prs.slide_layouts[1]  # Título y contenido
    slide = prs.slides.add_slide(slide_layout)
    slide.shapes.title.text = title
    slide.placeholders[1].text = content

# Diapositivas
add_slide(
    "Diseño de Red IPv6 para el Hospital General de Salud",
    "Nombre: Jefferson Gómez Guman\nPrograma académico: [Nombre del programa]\nCorreo institucional: [correo@unad.edu.co]\nObjetivo: Diseñar una red moderna para el Hospital General de Salud que integre IPv6, HCE, telemedicina, IoT y Wi-Fi para el personal médico."
)
add_slide(
    "Conceptos clave para la integración tecnológica",
    "- Tipos de redes: Guiadas y no guiadas\n- Ciclo de vida: Análisis, diseño, implementación, operación, mantenimiento, retiro\n- 4G/5G: Velocidad y baja latencia\n- IoT y redes inteligentes\n- IPv6: Seguridad y direccionamiento"
)
add_slide(
    "Necesidades técnicas y funcionales",
    "- Comunicación interna\n- Historia Clínica Electrónica\n- Seguridad y respaldo\n- Soporte IoT\n- Red Wi-Fi para personal"
)
add_slide(
    "Topología lógica de la red",
    "- 6 subredes: Urgencias, Consultas, Laboratorio, Farmacia, Administración, Wi-Fi\n- IPv6 base: 2001:DB8:ACAD::/48\n- Elementos: Routers, switches, servidores, IoT"
)
add_slide(
    "Servicios tecnológicos implementados",
    "- Servidor Web: Página institucional\n- Correo electrónico: @hospital.com\n- IoT: Sensores\n- Wi-Fi: Dispositivos médicos conectados"
)
add_slide(
    "Resultados y próximos pasos",
    "- Red funcional\n- Servicios activos\n- Comunicación verificada\n- Fases del ciclo de vida completas"
)

prs.save("Presentacion_Proyecto_Hospital_General_Jefferson.pptx")

