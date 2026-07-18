# 🤖 Especificación del hardware de código abierto de reBot DevArm


<p align="center">
  <img src="../../media/RS5_56.png" alt="Banner de reBot-DevArm">
</p>
<p align="center">
  <strong>
    <a href="./README_zh.md">简体中文</a> &nbsp;|&nbsp;
    <a href="./README.md">English</a> &nbsp;|&nbsp;
    <a href="./README_fr.md">français</a>&nbsp;|&nbsp;
    <a href="./README_es.md">Español</a>
  </strong>
</p>


| Fecha | Versión | Nombre del fichero | Registro de cambios |
|----------|------|----------|------|
|  2026-07-09 | v1.0 |  reBot_B601_RS_v1.0_20260625.step  | Publicación inicial |


Esta BOM corresponde al brazo robótico reBot Arm B601 RS, que utiliza motores de la serie RobStride. La otra versión, reBot Arm B601 DM, utiliza motores DAMIAO; [consulta la BOM aquí](../reBot_B601_DM/readme.md).

# 📦 Estructura de ficheros
*   3D_Printed_Parts/: ficheros STEP de todas las piezas impresas en 3D.
*   Metal_Parts/: ficheros STEP de todas las piezas metálicas mecanizadas por CNC.
*   Purchased_Parts/: ficheros STEP de todos los componentes comprados.
*   reBot_B601_RS_v1.0_20260625.step: fichero de ensamblaje completo del brazo robótico.

# 🛒 [Consigue todas las piezas](https://www.seeedstudio.com/reBot-Arm-B601-RS-Disassembly-Kit-Version-with-Power-Supply-Bundle.html)
- Ofrecemos cinco opciones de kit:
  - **reBot-Arm-B601-RS-Disassembly-Kit**
  - **reBot-Arm-B601-RS-Assembly-Version**

# 📊 Lista de materiales (BOM)

> [!WARNING]
> Aviso: la BOM publicada **no** representa la versión final que envía Seeed. Esta versión de código abierto v1.0 está optimizada para que los desarrolladores puedan reproducirla con el mínimo coste, con algunos detalles no esenciales simplificados.
> La versión final de producción de Seeed incluirá grabado láser en las piezas metálicas como sistema antierrores, algunas piezas impresas en 3D se sustituirán por metal para mayor durabilidad, las holguras y tolerancias de mecanizado se ajustarán en función de la variación de fábrica (equilibrando precisión y coste) y se añadirá cableado a medida (p. ej., protección con funda trenzada) con coste adicional. No obstante, la estructura mecánica sigue siendo idéntica.

---

## 🖨️ Piezas impresas en 3D

| Descripción de la pieza | Imagen | Nombre del fichero | Material | Cant. | Notas |
|----------|------|--------|------|----------|------|
| Plataforma de la base del brazo robótico | <img src="./3D_Printed_Parts/images/02-BASE.png" width="80"> | 1-BASE-PLATE.step | Bambu ABS negro | 1 | boquilla 0.4, altura de capa 0.2, relleno 30% |
| Eslabón de la base del brazo robótico | <img src="./3D_Printed_Parts/images/02-BASE_02.png" width="80"> | 1-RSM1-STATOR-1.step | Bambu ABS negro | 1 | boquilla 0.4, altura de capa 0.2, relleno 30% |
| Relleno izquierdo del brazo superior | <img src="./3D_Printed_Parts/images/02-DOWN_TRIM_1.png" width="80"> | 1-DOWN-DL.step | Bambu PLA negro y verde | 1 | boquilla 0.4, altura de capa 0.2, relleno 15% |
| Relleno derecho del brazo superior | <img src="./3D_Printed_Parts/images/02-DOWN_TRIM_2.png" width="80"> | 1-DOWN-DR.step | Bambu PLA negro y verde | 1 | boquilla 0.4, altura de capa 0.2, relleno 15% |
| Relleno central del brazo superior y del antebrazo | <img src="./3D_Printed_Parts/images/02-DOWN-FILLING.png" width="80"> | 1-SPACE-UP.step | Bambu ABS negro | 2 | boquilla 0.4, altura de capa 0.2, relleno 30% |
| Asa del brazo | <img src="./3D_Printed_Parts/images/02-HANDLE.png" width="80"> | 1-HANDLE.step | Bambu ABS negro | 1 | boquilla 0.4, altura de capa 0.2, relleno 30% |
| Cubierta del brazo superior y del antebrazo | <img src="./3D_Printed_Parts/images/02-DOWN-COVER.png" width="80"> | 1-COVER.step | Bambu PLA verde | 2 | boquilla 0.4, altura de capa 0.2, relleno 15% |
| Relleno izquierdo del antebrazo | <img src="./3D_Printed_Parts/images/02-UP-TRIM_1.png" width="80"> | 1-UP-DL.step | Bambu PLA negro y verde | 1 | boquilla 0.4, altura de capa 0.2, relleno 15% |
| Relleno derecho del antebrazo | <img src="./3D_Printed_Parts/images/02-UP-TRIM_2.png" width="80"> | 1-UP-DR.step | Bambu PLA negro y verde | 1 | boquilla 0.4, altura de capa 0.2, relleno 15% |
| Tope horizontal de la pinza (gripper) | <img src="./3D_Printed_Parts/images/02-SPACER.png" width="80"> | 1-STOPPER-1.step | Bambu PLA verde | 1 | boquilla 0.4, altura de capa 0.2, relleno 15% |
| Soporte del deslizador de la pinza | <img src="./3D_Printed_Parts/images/02-3D-RAIL-BRACKET.png" width="80"> | 1-RAIL-BASE-2.step | Bambu PLA verde | 1 | boquilla 0.4, altura de capa 0.2, relleno 15% |
| Dedo de la pinza | <img src="./3D_Printed_Parts/images/02-CLIP_1.png" width="80"> | 1-CLIP.step | Bambu ABS negro | 2 | boquilla 0.4, altura de capa 0.2, relleno 45%. Imprímelo apoyado sobre el lateral de la pinza para mejorar su resistencia estructural. |


El arrastre prolongado del arnés de cableado del motor 1 puede desgastar el conector del motor y provocar un mal contacto eléctrico. Imprimir las piezas que se indican a continuación puede mitigar este riesgo.

| Descripción de la pieza | Imagen | Nombre del fichero | Material | Cant. | Notas |
| ---- | ---- | ---- | ---- | ---- | ---- |
| Clips de arnés de cableado para ambos lados del motor 1 | <img src="./3D_Printed_Parts/images/RS_Motor1_wiring_harness_clip.jpg" width="80"> | `RS_Motor1_wiring_harness_clip.stp` | ABS negro Bambu Lab | 2 | boquilla de 0.4 mm, altura de capa 0.2 mm, relleno 30% |

### 🧩 Recomendaciones de impresión
- Altura de capa: 0.2 mm
- Boquilla: 0.4 mm
- Soportes: añadir según sea necesario
- Materiales: las piezas sometidas a altas temperaturas y a carga utilizan ABS con un relleno del 30–80%; también puede usarse nailon o materiales reforzados con fibra de carbono. Las piezas estéticas utilizan PLA con un relleno del 15%.

---

## 🔩 Piezas metálicas mecanizadas por CNC

> [!WARNING]
> Algunas piezas que pueden sustituirse por impresión 3D se indican en las notas, lo que puede reducir considerablemente los costes.

| Descripción de la pieza | Imagen | Nombre del fichero | Material | Cant. | Mecanizado | Notas |
|----------|------|--------|----------|------|------|------|
| Soporte del rodamiento del motor 1 | <img src="./Metal_Parts/images/02_Base_Reinforcement_Part.png" width="80"> | 2-RSM1-ROTOR-1.step | Aleación de aluminio 5052 | 1 | CNC |  |
| Pieza metálica izquierda del Link1 | <img src="./Metal_Parts/images/Link1_Left_Metal.png" width="80"> | 2-RSM-ROTOR-L.step | Aleación de aluminio 5052 | 1 | CNC |  |
| Pieza metálica derecha del Link1 | <img src="./Metal_Parts/images/Link1_Right_Metal.png" width="80"> | 2-RSM-ROTOR-R.step | Aleación de aluminio 5052 | 4 | CNC ||
| Pieza metálica inferior del Link1 | <img src="./Metal_Parts/images/Link1_Bottom_Metal.png" width="80"> | 2-RSM1-ROTOR-1.step | Aleación de aluminio 5052 | 3 | CNC | |
| Disco metálico de la articulación  | <img src="./Metal_Parts/images/2-CD.png" width="80"> | 2-CD.step | Aleación de aluminio 5052 | 3 | CNC | Se utiliza para ocultar los tornillos |
| Extensión frontal del RS06 | <img src="./Metal_Parts/images/RS06_Front_Extesnion.png" width="80"> | 2-RSM2-STATOR-1.step | Aleación de aluminio 5052 | 1 | CNC | |
| Extensión trasera del RS06 | <img src="./Metal_Parts/images/RS06_Back_Extesnion.png" width="80"> | 2-RSM2-STATOR-2.step | Aleación de aluminio 5052 | 1 | CNC | |
| Piezas metálicas izquierda y derecha del Link2 | <img src="./Metal_Parts/images/2-LINK-2_3.png" width="80"> | 2-LINK-2_3.step | Aleación de aluminio 5052 | 2 | CNC | |
| Tope superior L | <img src="./Metal_Parts/images/Upper_limit_L.png" width="80"> | 2-Upper-Limit_L.stp | Aleación de aluminio 5052 | 1 | CNC | |
| Tope superior R | <img src="./Metal_Parts/images/Upper_limit_R.png" width="80"> | 2-Upper-Limit_R.stp | Aleación de aluminio 5052 | 1 | CNC | |
| Unión de antebrazo y brazo superior L | <img src="./Metal_Parts/images/2-RSM3-ROTATOR-L.png" width="80"> | 2-RSM3-ROTATOR-L.step | Aleación de aluminio 5052 | 1 | CNC | |
| Unión de antebrazo y brazo superior R | <img src="./Metal_Parts/images/2-RSM3-ROTATOR-R.png" width="80"> | 2-RSM3-ROTATOR-R.step | Aleación de aluminio 5052 | 1 | CNC | |
| Pieza metálica izquierda del Link3 | <img src="./Metal_Parts/images/Link3-Left-Metal.png" width="80"> | 2-LINK-3_4-L.step | Aleación de aluminio 5052 | 1 | CNC | |
| Pieza metálica derecha del Link3 | <img src="./Metal_Parts/images/Link3-Right-Metal.png" width="80"> | 2-LINK-3_4-R.step | Aleación de aluminio 5052 | 1 | CNC | |
| Unión izquierda y derecha del Link3 | <img src="./Metal_Parts/images/Link3-Right-Left-Link.png" width="80"> | 2-SPACE-UP-2.step | Aleación de aluminio 5052 | 1 | CNC | |
| Fijación de cables de los motores 4-7 | <img src="./Metal_Parts/images/Motor4_Cable_Fixing.png" width="80"> | 1-O-CLIP.step | Aleación de aluminio 5052 | 4 | CNC | Seeed Studio envía esta pieza como un único componente metálico mecanizado por CNC integrado con otra pieza, lo que encarece la fabricación. Si reproduces el hardware por tu cuenta, puedes imprimir esta pieza en 3D con ABS e instalar tuercas M2 en las posiciones marcadas con las flechas rojas. |
| Link4-5_L | <img src="./Metal_Parts/images/Link4-5_L.png" width="80"> | 2-LINK-4_5-L.step | Aleación de aluminio 5052 | 1 | CNC | |
| Link4-5_R | <img src="./Metal_Parts/images/Link4-5_R.png" width="80"> | 2-LINK-4_5-R.step | Aleación de aluminio 5052 | 1 | CNC | |
| Link5 | <img src="./Metal_Parts/images/Link5.png" width="80"> | 2-RSM5-STATOR.step | Aleación de aluminio 5052 | 1 | CNC | |
| Conector de muñeca A | <img src="./Metal_Parts/images/Wrist_Connector_A.png" width="80"> | 2-RSM6-RORATOR-1.step | Aleación de aluminio 5052 | 1 | CNC |  |
| Conector de muñeca B | <img src="./Metal_Parts/images/Wrist_Connector_B.png" width="80"> | 2-RSM6-RORATOR-2.step | Aleación de aluminio 5052 | 1 | CNC |  |
| Conector de pinza A | <img src="./Metal_Parts/images/02_Gripper_Connector_A.png" width="80"> | 2-M6-ROTOR.step  | Aleación de aluminio 5052 | 1 | CNC | |
| Conector de pinza B | <img src="./Metal_Parts/images/02_Gripper_Connector_B.png" width="80"> | 2-M7-STATOR.step  | Aleación de aluminio 5052 | 1 | CNC | |
| Soporte metálico del deslizador de la pinza | <img src="./Metal_Parts/images/02_Slider_Bracket.png" width="80"> | 2-RAIL-BASE-1.step | Aleación de aluminio 5052 | 1 | CNC | Puede imprimirse en 3D en ABS con un relleno alto; no se recomienda para un uso prolongado |
| Extensión del deslizador a la pinza | <img src="./Metal_Parts/images/02_Slider_Extension.png" width="80"> | 2-SLIDER-FIX.step | Aleación de aluminio 5052 | 2 | CNC | |
| Cremallera | <img src="./Metal_Parts/images/Rack.png" width="80"> | 2-RACK-1M.step | Aleación de aluminio 5052 | 2 | CNC | |


### 🧩 Especificaciones de mecanizado
- Tolerancia de las dimensiones críticas: ±0.02 mm GB/T1840-M
- Acabado superficial: anodizado / arenado
- Ajuste recomendado para las piezas de acoplamiento: H7 (ajuste con apriete / por interferencia)
---

## 🛒 Piezas compradas (piezas estándar)

> [!WARNING]
> Dado que tendrás que montar y apretar los tornillos por tu cuenta, se han seleccionado tornillos Allen (de cabeza hexagonal interior) estándar. Tras un funcionamiento prolongado, los tornillos pueden aflojarse, lo que afectará a la precisión del brazo robótico. Por este motivo, es necesario que compres además pegamento termofusible para fijar la rosca de los tornillos de cada articulación.

Si dispones de un taladro eléctrico o de herramientas similares, puedes optar por comprar arandelas de bloqueo o tornillos con freno de rosca. No obstante, **es extremadamente importante** que utilices el ajuste de par más bajo del atornillador eléctrico para evitar pasar de rosca los tornillos, lo que provocaría daños irreversibles.


  | Nombre | Especificación / modelo | Cant. | Precio de referencia | Notas |
  |------|----------|------|----------|------|
  | Motor sin escobillas | RobStride RS00 | 4 | 125 $/unidad | [Seeed Studio](https://www.seeedstudio.com/Robostride-00-Actuator-p-6664.html) |
  | Motor sin escobillas | RobStride RS06 | 3 | 210 $/unidad |  [Seeed Studio](https://www.seeedstudio.com/Robostride-06-Actuator-p-6668.html)  |
  | Placa controladora CAN-USB |  | 1 | 15 $/unidad |   [Seeed Studio](https://www.amazon.com/Xiusiyt-Converter-Preloaded-PCAN-Firmware/dp/B0GBW7RTXD/ref=sr_1_2?crid=UNQHGEOCWEW4&dib=eyJ2IjoiMSJ9.BLjBmjTT73o_0hvb0ehHo3M2x1HYsciLqAZy-tlc_uo2eQn5T3jiElnghuDt__xr44HPQx8PITdTIyUG2aWDLwwAktkkejQPPmBc1dzKJXtZrK85hqgBHwCYeY-d8flD_XqsGw94kntXSOp-YSFCBZs-mBO2zVKZuQ6r_JoTjpZHNdDgWz9kMXtI7InFWPrKfV43IkBVJ6gssLjPd9ewBZyYVLORxBKVA6loljry6s1oEOVNtS3ChuU1bMmFcJNrZYlIJp0hqQkzS8kUxo3YIUQsO0GsdaxgyAIP2dpPNdw.O_Y2ZhdC1FWJ-A2gPo5jJHdw92tFf5LuHE9-oElawpA&dib_tag=se&keywords=Pcan&qid=1783575578&sprefix=pcan%2Caps%2C631&sr=8-2)   |
  | Placa de separación de alimentación XT30 2+2 |  | 1 | 15 $/unidad |   [Seeed Studio](https://www.seeedstudio.com/XT30-2-2-Power-Separation-Board-p-6707.html)   |
  | Rodamiento | 6803ZZ | 3 | 13 $/unidad | [Amazon](https://www.amazon.com/uxcell-17x26x5mm-Shielded-Precision-Lubricated/dp/B0D54JSWBZ/ref=sr_1_1?crid=17L94NDI1JCC0&dib=eyJ2IjoiMSJ9.xH_s9Ui7VlS40EZvr-HektqY3VOJsM-VjyE6JaJEScIWuFZ2UYSM7G8j1fC0HSmbb7YlA0YfUxxCkUzBptwrEEdEHsP94TGplNpPAWwhnH8b76HapXR_uHbr1vu3xe0AYSYP30Quk9LMQrGjUh84bXL82z2mORuiri0VHqo5DmSguK0cHubmVaXtbR_eJ43Z7L2nNqWfgltqzmHsYm7DQvrnIBg9UMlD1o9559nCSKA.E_N7CDPQhShckT-1vHDhYvNgiqRKusa12d43hqATQ5A&dib_tag=se&keywords=6803ZZ&qid=1774771801&sprefix=6803zz%2Caps%2C397&sr=8-1) |
  | Rodamiento | AXK5578 | 1 | 12 $/unidad | [Amazon](https://www.amazon.com/PZRT-AXK5578-Thrust-Bearings-Washers/dp/B0B3M3RZGW/ref=sr_1_1?dib=eyJ2IjoiMSJ9.TatYkzOvpYAJ5K23C7Qr9JKJsPhpJE8p1L3k5_1YqQ7ozSLNgOBEeG9pTYz-WXOWiHkbJq_zZR4FxNHAJZ4euyfOGXkOKycOyN0pUD0_WkJia0PekbRy0sYvyQbE7KZByR-40WiPSPuUcysFewSngPoDGQZzESFOUz__V9ViGCIQAPfdUe2OxVpvtbKZYCQsrSDm8b8okR25bavCvpDbBfPh0He2PEBEpl55L8RtYKmlv62XJyfYT1o29A7wO5n8-g3hpJOrKmmWCybdEEWSmquAT1cjvsPTJDaT_TICsso.6xR5pEGJgTR-u_NOyXxi8VTphoLytGd8zugy1-xu-fE&dib_tag=se&keywords=AXK5578&qid=1774771826&sr=8-1&th=1) |
  | Raíl lineal | MGN9-170mm | 1 | 23 $/unidad | [Amazon](https://www.amazon.com/uxcell-Sliding-Carriage-Bearing-Printers/dp/B0D54L45WM/ref=sr_1_1?dib=eyJ2IjoiMSJ9.qNphfY5r4UgLDHslIliMBhC45qBKTl37lJseObJSBp79RJ4VJnAH-lYAMo-rwPiu_uqWmkN7ms4kfAokYvod1seWb5-z2_kVgVuzrCXdiRycNXjrdv3qi5Awuno0_vEqjT4WJ569tAmqm_Rujrdxss7VfpLizFxq6-R8DucuvqZ0M0Y4go9PzRFEFPu4csskz7-UkM1CUidHoKmrT-I7R1Ta0dijj2SYlR_zW0si75k.nRJTebbqw-bFyzkdU8MztHnGdt9qwnHr_gIqa-MDxEQ&dib_tag=se&keywords=MGN9&qid=1774771864&sr=8-1) |
  | Bloque deslizante | MGN9 | 2 | 10 $/unidad | [Amazon](https://www.amazon.com/uxcell-Bearing-Sliding-Carriage-Anti-Fall/dp/B0D9QBQDKB/ref=sr_1_8?dib=eyJ2IjoiMSJ9.qNphfY5r4UgLDHslIliMBhC45qBKTl37lJseObJSBp79RJ4VJnAH-lYAMo-rwPiu_uqWmkN7ms4kfAokYvod1seWb5-z2_kVgVuzrCXdiRycNXjrdv3qi5Awuno0_vEqjT4WJ569tAmqm_Rujrdxss7VfpLizFxq6-R8DucuvqZ0M0Y4go9PzRFEFPu4csskz7-UkM1CUidHoKmrT-I7R1Ta0dijj2SYlR_zW0si75k.nRJTebbqw-bFyzkdU8MztHnGdt9qwnHr_gIqa-MDxEQ&dib_tag=se&keywords=MGN9&qid=1774771864&sr=8-8) |
  | Engranaje | Módulo 1, tipo con cubo, 16 dientes, agujero de 6 mm | 1 | 44 $/unidad | [Amazon](https://www.amazon.com/Module-15-Teeth-Finished-Perforation/dp/B0GDSR1LKM/ref=sr_1_1?crid=2EN1YHE8TEC58&dib=eyJ2IjoiMSJ9.54N73iSlush8K1a_teRazjBGZaQnbFM4MLysEbIq430CEYcVs0slm8KhpC_JlmjyVMocPA3vLANjERYZWweRag36NhX2GGldVTpd31kAWW4.ws8l0qBABmSVrUGX4g2o3sBbUgOnNhl3Nx_Nt-d1HT8&dib_tag=se&keywords=1%2Bmodule16%2Bteeth&qid=1774772022&sprefix=1%2BModule16%2Bteeth%2Caps%2C403&sr=8-1&th=1)  |
  | Almohadilla de silicona | 30 × 9 × 2 mm | 1 | 10 $ | [Amazon](https://www.amazon.com/Self-Adhesive-Anti-Sliding-Anti-Scratch-Protectors-Appliances/dp/B0F9KVYXFZ/ref=sr_1_3?crid=LVY2LLBFQT6J&dib=eyJ2IjoiMSJ9.4qjOEtjEph1QxS_kJF2vIYqvD_8Lzt4GZ2rrywWbrAhniBvp_8YrEsVNcCPQofO4jVqBxFE8Yplyg2XXgAXlUZwzqE-Gp8MYcaPmphL8Mc1n-ARSCNaTq5gc7ZIWsS6u-kR0G2BzIlBo6NF88KvASjKYJfTHpPXHfNCPVw13P-PseVbUZwlVAO9zMHa3a84gHRd-I-mGB8SCmek9mXjN-c-bFxKvJXlz4C5YBBdt9cH3QkSmLgiLZ_iD4K1mh-MwI5WuVOXr5ZOwJ0bVpmHpc_vpbKLr7CkVack3nsC-TM0.40ujhwS5ConOfA8io_c5hcdos70HOKjMFqqKLKgNwI8&dib_tag=se&keywords=silicone%2Bsticker&qid=1774772199&sprefix=silicone%2Bsticker%2Caps%2C380&sr=8-3&th=1) |
  | Tornillo | Tornillo KM3*7mm | 80+ |  |[Amazon](https://www.amazon.com/Uxcell-a16011300ux0872-M3x12mm-Carbon-Countersunk/dp/B01E6EIC2S/ref=sr_1_1?crid=2VJKS347LBDWD&dib=eyJ2IjoiMSJ9.eXF2FHahloRY0Kq8sM_EkJUm7ipUgMoVSuTAPjt3ZnAINqLrPQz9A55XDHfe00KPGG3Sr1IJJQloiw7IFwewoPsbdnKBZH5JjT4Ijy_bUXju1IvrHWP4nWeYW1o29jlbHBKEa3fPl8-JzEHr9RPKe5h_Dr1vN6VFMUfszTDEzufQrIi22AsKCMTep5n0-IR7AIc7Fai93nmr4ax8USKGOD_3yu4ri0p8ClPTZzfwmDJvnTpE9J9PNN8uA-wDz72RADQu2VLry_mvb5CA1JV0vHP49Qsy-96MKXo-j3vT8m0.DWiT1Loy7A-MeTveRzxU47S6WCKwnW6MVnmpF256j-s&dib_tag=se&keywords=screw+KM3*12&qid=1776330785&s=industrial&sprefix=screw+km3+%2Cindustrial%2C984&sr=1-1)   |
  | Tornillo | Tornillo KM3*16mm | 8+ |  |[Amazon](https://www.amazon.com/Uxcell-a16011300ux0872-M3x12mm-Carbon-Countersunk/dp/B01E6EIC2S/ref=sr_1_1?crid=2VJKS347LBDWD&dib=eyJ2IjoiMSJ9.eXF2FHahloRY0Kq8sM_EkJUm7ipUgMoVSuTAPjt3ZnAINqLrPQz9A55XDHfe00KPGG3Sr1IJJQloiw7IFwewoPsbdnKBZH5JjT4Ijy_bUXju1IvrHWP4nWeYW1o29jlbHBKEa3fPl8-JzEHr9RPKe5h_Dr1vN6VFMUfszTDEzufQrIi22AsKCMTep5n0-IR7AIc7Fai93nmr4ax8USKGOD_3yu4ri0p8ClPTZzfwmDJvnTpE9J9PNN8uA-wDz72RADQu2VLry_mvb5CA1JV0vHP49Qsy-96MKXo-j3vT8m0.DWiT1Loy7A-MeTveRzxU47S6WCKwnW6MVnmpF256j-s&dib_tag=se&keywords=screw+KM3*12&qid=1776330785&s=industrial&sprefix=screw+km3+%2Cindustrial%2C984&sr=1-1)   |
  | Tornillo | KA3*12mm | 48+ |  | [Amazon](https://www.amazon.com/uxcell-Phillips-Tapping-Screws-Silver/dp/B01MXSS95N/ref=sr_1_3?crid=2RJ5ZBG0M4EX5&dib=eyJ2IjoiMSJ9.v9AtN0DrK0YdOT84Puh29n1VDClJz4OwvslbH610w0_xJIkuVFk81UxgSw_lSRbHugpqkja4rz-elY-DHbh0KN4GCFH2MlZhRFjXVE1vlaChALTqgr9jxatNPvPTf8SzdxFoEMEPm3jwCnC8vqLq5xL-Wr414hMsTbVYxv_ZVmEbMV-8YYXhLWiOz9EivU2C8jWw0RFSwVtUxqhj7qgBBYV5QbJRNr1XdWmQsICMHTHy35DeIcLjyKtXOb0gEwDNyqqmdvS5LfJJaLQchjLpW1jondo5xapQVw8gWJ4yYjk.oXwiRL9W52Tlu7tMi7tT9i7g-CBYfw_AAT1LURe2Q7k&dib_tag=se&keywords=screw+ka3*12&qid=1776331569&s=industrial&sprefix=screw+ka3+%2Cindustrial%2C466&sr=1-3)  |
  | Tornillo | Tornillo HM3-8mm | 60+ |  | [Amazon](https://www.amazon.com/BNUOK-120pcs-Stainless-Threads-Spanner/dp/B0DJQG5YLF/ref=sr_1_4?crid=3J1D711FNBYR9&dib=eyJ2IjoiMSJ9.wo20uXEJsuYS5OBVpnH9TILDd6HtQrJUlEvvYFPE5VV6bozIiRlWwmDaoYnp345KjXwRyxbEgEaRD8gVD2vVhPXg3M266n3H8t9cWN518aR4c5WkFUkqLIqLwdGYBllKcQQ8agsrZYgSVFp9G8LJR4l9oAj8Yx4QN8MReo2k23RVk-lkWeJk1azXD88GFTmd17aiXz6fwOE45Krj4VRiy1oskx8QvMprmJXtH8KowAJo-pWdBtePCCIUUa8oLR78hi17yW_OGJattIwdAziX9RizLI-EMh3hku42WJWnb3g.lZYqsYfJunSoEUPNT04E1sFhPiudREmrI0919PaPBYI&dib_tag=se&keywords=screw%2BHM3-12mm&qid=1776330531&s=industrial&sprefix=screw%2Bhm3-12mm%2Cindustrial%2C475&sr=1-4&th=1)  |
  | Tornillo | Tornillo HM3-30mm | 16+ |  | [Amazon](https://www.amazon.com/BNUOK-120pcs-Stainless-Threads-Spanner/dp/B0DJQFGRPQ/ref=sr_1_4?crid=3J1D711FNBYR9&dib=eyJ2IjoiMSJ9.wo20uXEJsuYS5OBVpnH9TILDd6HtQrJUlEvvYFPE5VV6bozIiRlWwmDaoYnp345KjXwRyxbEgEaRD8gVD2vVhPXg3M266n3H8t9cWN518aR4c5WkFUkqLIqLwdGYBllKcQQ8agsrZYgSVFp9G8LJR4l9oAj8Yx4QN8MReo2k23RVk-lkWeJk1azXD88GFTmd17aiXz6fwOE45Krj4VRiy1oskx8QvMprmJXtH8KowAJo-pWdBtePCCIUUa8oLR78hi17yW_OGJattIwdAziX9RizLI-EMh3hku42WJWnb3g.lZYqsYfJunSoEUPNT04E1sFhPiudREmrI0919PaPBYI&dib_tag=se&keywords=screw%2BHM3-12mm&qid=1776330531&s=industrial&sprefix=screw%2Bhm3-12mm%2Cindustrial%2C475&sr=1-4&th=1) |
  | Tornillo | Tornillo prisionero HM4-8mm | 6+ |  | [Amazon](https://www.amazon.com/iexcell-Partially-Threaded-Thread-Socket/dp/B0DR1NX178/ref=sr_1_1?crid=35DT1MLQCOR9C&dib=eyJ2IjoiMSJ9.RlFuoSyG6Yoi2cmVkd0sQ47UpPY4y8uvofyrje4Ha76Dj6dcpknwvFT7DGc5jFqxw5Zd5g4SV-yre7xcMb3WB7MbBowQO3ZzvCgpYWcJ2xzphgz9gx0SNIr_ggqvFcAmxkNuMMVf0p9vPY-jJ2j9cbIk8IwMHlTo6kkuBINPotouNNyElpiy9qHhllwajmKY5v5uDIzJKNJvmhpUtJsd5IS7TB9VaRPkzsDbMDfR4pvs4JgNbU1Zmcu4Ex9fYcRHrOGjAZbbvNxo1r_N5MBKWbxbtZEDDKP_8Oyhgakhhnc.MTLa-_9PBksy6Qge1YqQmlejVfLKkuxB9gT-ZnB9ek0&dib_tag=se&keywords=screw+HM4-75&qid=1776330730&s=industrial&sprefix=screw+m4-75%2Cindustrial%2C401&sr=1-1)  |
  | Tornillo | Tornillo prisionero HM4-16mm | 18+ |  | [Amazon](https://www.amazon.com/iexcell-Partially-Threaded-Thread-Socket/dp/B0DR1NX178/ref=sr_1_1?crid=35DT1MLQCOR9C&dib=eyJ2IjoiMSJ9.RlFuoSyG6Yoi2cmVkd0sQ47UpPY4y8uvofyrje4Ha76Dj6dcpknwvFT7DGc5jFqxw5Zd5g4SV-yre7xcMb3WB7MbBowQO3ZzvCgpYWcJ2xzphgz9gx0SNIr_ggqvFcAmxkNuMMVf0p9vPY-jJ2j9cbIk8IwMHlTo6kkuBINPotouNNyElpiy9qHhllwajmKY5v5uDIzJKNJvmhpUtJsd5IS7TB9VaRPkzsDbMDfR4pvs4JgNbU1Zmcu4Ex9fYcRHrOGjAZbbvNxo1r_N5MBKWbxbtZEDDKP_8Oyhgakhhnc.MTLa-_9PBksy6Qge1YqQmlejVfLKkuxB9gT-ZnB9ek0&dib_tag=se&keywords=screw+HM4-75&qid=1776330730&s=industrial&sprefix=screw+m4-75%2Cindustrial%2C401&sr=1-1)  |
  | Tornillo | Tornillo prisionero HM4-70mm | 4+ |  | [Amazon](https://www.amazon.com/iexcell-Partially-Threaded-Thread-Socket/dp/B0DR1NX178/ref=sr_1_1?crid=35DT1MLQCOR9C&dib=eyJ2IjoiMSJ9.RlFuoSyG6Yoi2cmVkd0sQ47UpPY4y8uvofyrje4Ha76Dj6dcpknwvFT7DGc5jFqxw5Zd5g4SV-yre7xcMb3WB7MbBowQO3ZzvCgpYWcJ2xzphgz9gx0SNIr_ggqvFcAmxkNuMMVf0p9vPY-jJ2j9cbIk8IwMHlTo6kkuBINPotouNNyElpiy9qHhllwajmKY5v5uDIzJKNJvmhpUtJsd5IS7TB9VaRPkzsDbMDfR4pvs4JgNbU1Zmcu4Ex9fYcRHrOGjAZbbvNxo1r_N5MBKWbxbtZEDDKP_8Oyhgakhhnc.MTLa-_9PBksy6Qge1YqQmlejVfLKkuxB9gT-ZnB9ek0&dib_tag=se&keywords=screw+HM4-75&qid=1776330730&s=industrial&sprefix=screw+m4-75%2Cindustrial%2C401&sr=1-1)  |
 | Tornillo | Tornillo HM3-6mm | 8+ |  | [Amazon](https://www.amazon.com/BNUOK-120pcs-Stainless-Threads-Spanner/dp/B0DJQG5YLF/ref=sr_1_4?crid=3J1D711FNBYR9&dib=eyJ2IjoiMSJ9.wo20uXEJsuYS5OBVpnH9TILDd6HtQrJUlEvvYFPE5VV6bozIiRlWwmDaoYnp345KjXwRyxbEgEaRD8gVD2vVhPXg3M266n3H8t9cWN518aR4c5WkFUkqLIqLwdGYBllKcQQ8agsrZYgSVFp9G8LJR4l9oAj8Yx4QN8MReo2k23RVk-lkWeJk1azXD88GFTmd17aiXz6fwOE45Krj4VRiy1oskx8QvMprmJXtH8KowAJo-pWdBtePCCIUUa8oLR78hi17yW_OGJattIwdAziX9RizLI-EMh3hku42WJWnb3g.lZYqsYfJunSoEUPNT04E1sFhPiudREmrI0919PaPBYI&dib_tag=se&keywords=screw%2BHM3-12mm&qid=1776330531&s=industrial&sprefix=screw%2Bhm3-12mm%2Cindustrial%2C475&sr=1-4&th=1)  |
 | Tornillo | Tornillo HM3-26mm | 6+ |  | [Amazon](https://www.amazon.com/BNUOK-120pcs-Stainless-Threads-Spanner/dp/B0DJQG5YLF/ref=sr_1_4?crid=3J1D711FNBYR9&dib=eyJ2IjoiMSJ9.wo20uXEJsuYS5OBVpnH9TILDd6HtQrJUlEvvYFPE5VV6bozIiRlWwmDaoYnp345KjXwRyxbEgEaRD8gVD2vVhPXg3M266n3H8t9cWN518aR4c5WkFUkqLIqLwdGYBllKcQQ8agsrZYgSVFp9G8LJR4l9oAj8Yx4QN8MReo2k23RVk-lkWeJk1azXD88GFTmd17aiXz6fwOE45Krj4VRiy1oskx8QvMprmJXtH8KowAJo-pWdBtePCCIUUa8oLR78hi17yW_OGJattIwdAziX9RizLI-EMh3hku42WJWnb3g.lZYqsYfJunSoEUPNT04E1sFhPiudREmrI0919PaPBYI&dib_tag=se&keywords=screw%2BHM3-12mm&qid=1776330531&s=industrial&sprefix=screw%2Bhm3-12mm%2Cindustrial%2C475&sr=1-4&th=1)  |
 | Cable XT30 2+2 | Codo en ambos extremos, 320 mm | 1+ |  <img src="./Metal_Parts/images/XT30.png" width="80"> | Debes fabricarlo a medida tú mismo.  |
 | Cable XT30 2+2 | Codo en ambos extremos, 200 mm | 4+ |  <img src="./Metal_Parts/images/XT30.png" width="80"> | Debes fabricarlo a medida tú mismo.  |
 | Cable XT30 2+2 | Codo en un extremo, 300 mm | 1+ |  <img src="./Metal_Parts/images/XT30.png" width="80"> |  Debes fabricarlo a medida tú mismo. |
 | Cable XT30 2+2 | Recto en ambos extremos | 1+ |  |   |
  | Juego de destornilladores | Juego de llaves hexagonales | 1 | 16 $  | [Amazon](https://www.amazon.com/Amazon-Basics-Ratcheting-Electronics-Screwdriver/dp/B07V4TFWFZ/ref=sr_1_2?crid=ADAY70RZDSLN&dib=eyJ2IjoiMSJ9.jcLL4o6IXTnPlPfTTzbCZCBuZx2sLkvdUQCwlL58aq__GOyLxVPnwLI0mvGptba_HeVz6ctLQ_ziQw56BMDH9IOaw-4PVJGMktQM74mWficwggm3ckDGyAH-agN_zkB3K0_W-wrS56jfcMYFbZSWhWxr-iSOC4sdXwMGlt4rYGtenyn9yAFYBIHqjU2El5_OAKuspsrF0yQvfyfQPQHs46SClWN8zlSemGVZRuVSU26f0f9yApF6BfWHANKNNhT0Mfb6bQ8oM2XUMvwaazrrKoHeTARuoflVaVZvMU776bs.r8gy_gMINEy0qy4JyK--z-IbPZEv-SWeMGohOOE7M60&dib_tag=se&keywords=Screwdriver+set&qid=1774772499&s=industrial&sprefix=screwdriver+set+%2Cindustrial%2C374&sr=1-2)  |



### Acerca de la fijación
Puedes modificar libremente la base a partir de las piezas impresas en 3D que proporcionamos. También puedes utilizar sargentos tipo G según el grosor de tu mesa.

  | Nombre | Especificación / modelo | Cant. | Precio de referencia | Notas |
  |------|----------|------|----------|------|
  | Sargento de carpintería | Sargento tipo G de 6 pulgadas | 2 | 20 $/unidad | [Amazon](https://www.amazon.com/gp/aw/d/B092J1YW2M/?_encoding=UTF8&pd_rd_plhdr=t&aaxitk=3557c048ce58e7dbb50b40c3af69f1d6&hsa_cr_id=0&qid=1774772748&sr=1-1-9e67e56a-6f64-441f-a281-df67fc737124&ref_=sbx_s_sparkle_sbtcd_asin_0_img&pd_rd_w=bNqtC&content-id=amzn1.sym.2fb72bc8-96ef-420d-b08f-c04b69f36507%3Aamzn1.sym.2fb72bc8-96ef-420d-b08f-c04b69f36507&pf_rd_p=2fb72bc8-96ef-420d-b08f-c04b69f36507&pf_rd_r=KDCPNZRHFWEWBWVHWSTR&pd_rd_wg=sBvfF&pd_rd_r=52b946ee-46e2-4e74-86ee-99e291552e44) |



### Acerca de la alimentación
El brazo robótico se envía por defecto sin fuente de alimentación. Puedes conectar tu propia batería o comprar una fuente de alimentación Mean Well fiable de 48 V y 12.5 A fabricada en Taiwán. Además, necesitarás comprar un enchufe de tres clavijas conforme a la normativa local y un arnés de cables con conector XT30 hembra.

#### BOM de consumibles

| Nombre | Especificación | Cant. | Precio de referencia | Notas | Imagen |
|:---|:---|:---:|:---:|:---|:---:|
| Fuente de alimentación | LRS-600-48 (48 V, 12.5 A) | 1 | 69.5 $ | [amazon](https://www.amazon.com/LRS-600-48-Switching-Upgrade-Version-SE-600-48/dp/B0BV5XFYNS/ref=sr_1_1?crid=2MK5Y1UI66CW9&dib=eyJ2IjoiMSJ9.FAt8rrpVeLIbeU2px5Bpe3WU2xsHpE3Kw1Fc6ZdPBFrIpRsaASOwU1dL9jPUNnpXO5u67hvlSXTsKCXH7jehZ8VWfiSFbcHmsVhJY_ua86iPUltJFeWlT9LIXphFER27jHWGnaJb2NdRIpPBMVdae8qgIllUI1J-Q8pZranpyjkkiJP2RmiEdhUBXTvvH3-vhk8z2uhf7BJrGW7hjRbjyCO7WHwwBQ3tMcnEKwto2doy9qus35djHRzODSFPbMuiA66PdgPuib4VL1aQghehDEiceMIpTUiCHHeRHfpB71M._yrosm8mVfpUq-5PjNTLSaYPgv8Dot6YbQTaGULjlLQ&dib_tag=se&keywords=LRS-600-48&qid=1781762081&s=electronics&sprefix=lrs-600-48%2Celectronics%2C351&sr=1-1) | <img src="./Purchased_Parts/LRS-600-48.png" width="80"> |
| Cable de alimentación | Cable de CA estándar de EE. UU. | 1 | 4.49 $ | [amazon](https://www.amazon.com/LIFEPOE-Power-3-3ft-Black-3-Prong/dp/B0FK4KPW2G/ref=sr_1_1?crid=2W5766PT8EOKA&dib=eyJ2IjoiMSJ9.7E5s-9-Zh-jJAdni-17Iyt1Mr3GJD6hMt9pfk-0S5YxZtknZik9OiePitwUom0pYUbePRpdqa0dCZtGUjluQDEJbSDePHCGvBV6bwQU7wfwd0Loo4WJJmH_2CM1KRKSPcxHXRH0i1i5yuy4g7fDxxn3nPGYU3aF00m5jiIkMfYFgOxH4yURjjZeTMZAIO9wiVQUsPrlM51UIgpPo2YYdCQVUsxjumSsTAm0Jpt2SsBEdT-QzXSIKpLSvQ6kGijXF-4ZevaxiShJdmwU8t2LobDLcalXEOl3lriZTGhjwxow.r0oBabUkGwewhvO3IKlBMULdhUSe6yNTsjfFUaBsjyU&dib_tag=se&keywords=US%2BStandard%2BAC%2BCable%3B%2B1.5m%2B-%2B3%2B*%2B1.5mm%C2%B2&nsdOptOutParam=true&qid=1780021862&s=industrial&sprefix=lrs-350-24%2Cindustrial%2C387&sr=1-1&th=1) | <img src="./Purchased_Parts/US Standard AC Cable.png" width="80"> |
| Puerto de salida | Conector hembra fijo XT60E; XT60E hembra + terminal de cable - 10 cm; agujero de terminal de 4 mm | 1 | 9.99 $ | [amazon](https://www.amazon.com/LINSYRC-XT60E-F-Connector-Battery-Quadcopter/dp/B0CQK1P1DP/ref=pd_sbs_d_sccl_1_2/133-3898271-3474923?pd_rd_w=FmCVA&content-id=amzn1.sym.aa738fbd-ad05-4d11-aae2-04b598db6305&pf_rd_p=aa738fbd-ad05-4d11-aae2-04b598db6305&pf_rd_r=03QM0MRVZA968N9X6X6E&pd_rd_wg=WOZ9q&pd_rd_r=6e0577d2-de73-4427-affd-a271808e1453&pd_rd_i=B0CQK1P1DP&psc=1) | <img src="./Purchased_Parts/XT60E Female to Copper Lug Pigtail.png" width="80"> |
| Cableado de CA de alimentación | 1.5 mm²; rojo, azul y amarillo, 1 de cada (debes crimpar tú mismo los terminales al cable; no se incluyen cables precrimpados); 10 cm | 3 | 0.99 $ | [aliexpress](https://www.aliexpress.com/item/1005008648016252.html?spm=a2g0o.productlist.main.2.15c9ZpluZpluHP&algo_pvid=09efee83-d80c-4ece-b588-3b1ef73279a3&algo_exp_id=09efee83-d80c-4ece-b588-3b1ef73279a3-1&pdp_ext_f=%7B%22order%22%3A%22230%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21USD%213.58%210.99%21%21%2124.09%216.65%21%400b0b305117800339070873795e0f3d%2112000046086542230%21sea%21US%216593543849%21ABX%211%210%21n_tag%3A-29910%3Bd%3A518b3f9d%3Bm03_new_user%3A-29895%3BpisId%3A5000000207178484&curPageLogUid=74aJ9L7lm7hs&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005008648016252%7C_p_origin_prod%3A&gatewayAdapt=4itemAdapt) | <img src="./Purchased_Parts/RV Grounding Wire Coil with Y-Terminal Lugs.png" width="80"> |
| Toma IEC 3 en 1 | Tipo de conexión rápida con interruptor rojo (doble tuerca) | 1 | 1.98 $ | [aliexpress](https://www.aliexpress.com/item/1005005962021242.html?spm=a2g0o.imagesearchproductlist.main.17.7db7cZZdcZZdCY&algo_pvid=270b0987-1973-41ad-a2b9-6fe008f9edb5&algo_exp_id=270b0987-1973-41ad-a2b9-6fe008f9edb5&pdp_ext_f=%7B%22order%22%3A%22346%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21USD%213.31%211.98%21%21%2122.30%2113.35%21%400b0b305117800327806706342e118f%2112000035062406338%21sea%21US%216593543849%21ABX%211%210%21n_tag%3A-29910%3Bd%3A518b3f9d%3Bm03_new_user%3A-29895%3BpisId%3A5000000204886261&curPageLogUid=87JUDbPbch2i&utparam-url=scene%3Aimage_search%7Cquery_from%3Apc_web_image_search%7Cx_object_id%3A1005005962021242%7C_p_origin_prod%3A) | <img src="./Purchased_Parts/3-in-1 IEC Inlet Socket.png" width="80"> |
| Cable adaptador XT30 a XT60 con conector, 12awg | XT30U hembra a XT60 macho, longitud del cable 50 cm | 1 | 9.98 $ | [amazon](https://www.amazon.com/MEIRIYFA-Extension-Female-Adapter-Silicone/dp/B0B3DMJVV8/ref=sr_1_27?crid=18IGT0X1XS48F&dib=eyJ2IjoiMSJ9.qYRdGYT8G-SZEIPj6hMxuQLGxfv2AtkCiY3gitqnCn5xQhGZdsRAFETuJHlWK8od694BVQ9S5s-Pj7SsVcJxjxrXykP4sit5Cmz2HvRUzULa_jT-oGoR0ErPyaatF5aedauUQmY5bi6aYn5K_820VyPI6Jc-7L18WxPv0MVWxPMSduUx-Wu_VatV1AdePPQQsG63GQJm-JbW1p6lDP5gP1PTfDeoTd17xzb3QaooEDkJ9ktKNAjACX9UP7-xnS-vN7HTzX9NWkcKM8Ce0mYer_h5tnweVDzKnZlP65KMXDM.OXhg6VlhBUozkydCUQvH5OTfWZVSK-RkVZ-D5apJWzY&dib_tag=se&keywords=XT30+XT-30+to+XT60+XT-60+Male+Female+RC+Connector+Adapter+with+16awg+30cm&nsdOptOutParam=true&qid=1780818603&sprefix=xt30+xt-30+to+xt60+xt-60+male+female+rc+connector+adapter+with+16awg+3cm%2Caps%2C520&sr=8-27) | <img src="./Purchased_Parts/XT30U_female_to_XT60_male.png" width="80"> |
| Tornillo Phillips de cabeza avellanada de acero inoxidable 304 | M4x6 | 10 | 0.37 $ | / | / |
| Tornillo Phillips de cabeza avellanada de acero inoxidable 304 | M3x8 | 2 | 0.36 $ | / | / |
| Tornillo Phillips de cabeza alomada de acero inoxidable 304 | M3x8 | 2 | 0.32 $ | / | / |
| Tuerca hexagonal | M3x2.5 | 2 | 2.10 CNY | / | / |

BOM de piezas impresas:

| Nombre | Imagen | Cant. | Notas |
| ------ | ---- | --- | ---- |
| [Carcasa frontal](./3D_Printed_Parts/RS-power-Top%20Cover.stp) | <img src="./3D_Printed_Parts/images/RS-power-Top Cover.png" width="80"> | 1 | PLA, boquilla 0.4, altura de capa 0.2, relleno 30% |
| [Carcasa trasera](./3D_Printed_Parts/RS-power-Bottom%20Cover.stp) | <img src="./3D_Printed_Parts/images/RS-power-Bottom Cover.png" width="80"> | 1 | PLA, boquilla 0.4, altura de capa 0.2, relleno 30% |
| [Carcasa frontal (tapa deslizante)](./3D_Printed_Parts/RS-power-Top%20Cover-Sliding%20Cover.stp) | <img src="./3D_Printed_Parts/images/RS-power-Top Cover-Sliding Cover.png" width="80"> | 1 | PLA, boquilla 0.4, altura de capa 0.2, relleno 30% |

#### Montaje de la fuente de alimentación

- Los pasos de montaje de la fuente de alimentación se dividen en dos partes: la carcasa frontal y la carcasa trasera.

##### 1. Montaje de la carcasa frontal

| Paso | Descripción | Imagen | Notas |
|:---:|---|---|---|
| 1-1 | Prepara las piezas y los componentes impresos necesarios para el montaje de la carcasa frontal | <img src="./Assembly_Steps/powerstep_images/1-1.png" width="80"> | Comprueba que están todas las piezas |
| 1-2 | Monta cada pieza siguiendo el orden de cableado indicado en las imágenes | <img src="./Assembly_Steps/powerstep_images/1-2(1).png" width="80" style="margin-right:4%;"><img src="./Assembly_Steps/powerstep_images/1-2(2).png" width="80"><br><img src="./Assembly_Steps/powerstep_images/1-2(3).png" width="80"> | Conecta siguiendo estrictamente el orden de cableado |
| 1-3 | Instala el conector XT60 | <img src="./Assembly_Steps/powerstep_images/1-3（1）.png" width="80" style="margin-right:4%;"><img src="./Assembly_Steps/powerstep_images/1-3（2）.png" width="80"> | Fíjalo con tornillos Phillips de cabeza avellanada M3x8 de acero inoxidable 304 y tuercas hexagonales M3x2.5 |
| 1-4 | Instala la toma IEC 3 en 1 | <img src="./Assembly_Steps/powerstep_images/1-4（1）.png" width="80" style="margin-right:4%;"><img src="./Assembly_Steps/powerstep_images/1-4（2）.png" width="80"> | Fija la toma IEC 3 en 1 con tornillos Phillips de cabeza alomada M3x8 de acero inoxidable 304 |
| 1-5 | Cableado interno de la carcasa frontal | <img src="./Assembly_Steps/powerstep_images/1-5（1）.png" width="80"><br><img src="./Assembly_Steps/powerstep_images/1-5（2）.png" width="80"> | Comprueba las conexiones según el esquema de cableado |
| 1-6 | Fija la carcasa frontal a ambos lados de la fuente de alimentación | <img src="./Assembly_Steps/powerstep_images/1-6（1）.png" width="80" style="margin-right:4%;"><img src="./Assembly_Steps/powerstep_images/1-6（2）.png" width="80"> | 4 tornillos Phillips de cabeza avellanada M4x6 de acero inoxidable 304 |
| 1-7 | Instala la tapa deslizante | <img src="./Assembly_Steps/powerstep_images/1-7（1）.png" width="80" style="margin-right:4%;"><img src="./Assembly_Steps/powerstep_images/1-7(2).png" width="80"> | Introdúcela desde la parte inferior de la fuente de alimentación |
| 1-8 | Fija la tapa deslizante | <img src="./Assembly_Steps/powerstep_images/1-8.png" width="80"> | 2 tornillos Phillips de cabeza avellanada M4x6 de acero inoxidable 304 |

---

##### 2. Montaje de la carcasa trasera

| Paso | Descripción | Imagen | Notas |
|:---:|---|---|---|
| 2-1 | Prepara las piezas y los componentes impresos necesarios para el montaje de la carcasa trasera | <img src="./Assembly_Steps/powerstep_images/2-1.png" width="80"> | Comprueba que todos los accesorios están completos |
| 2-2 | Ensambla la carcasa trasera con la fuente de alimentación | <img src="./Assembly_Steps/powerstep_images/2-2.png" width="80"> | Alinea la posición |
| 2-3 | Fija la carcasa trasera a ambos lados de la fuente de alimentación | <img src="./Assembly_Steps/powerstep_images/2-3(1).png" width="80" style="margin-right:4%;"><img src="./Assembly_Steps/powerstep_images/2-3(2).png" width="80"> | 4 tornillos Phillips de cabeza avellanada M4x6 de acero inoxidable 304 |

---

##### 3. Finalización

| Paso | Descripción | Imagen | Notas |
|:---:|---|---|---|
| 1 | Montaje de la fuente de alimentación completado | <img src="./Assembly_Steps/powerstep_images/3.png" width="80"> | Comprueba que todos los tornillos están bien apretados |

---
