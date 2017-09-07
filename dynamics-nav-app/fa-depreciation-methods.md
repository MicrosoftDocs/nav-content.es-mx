---
title: "Métodos de depreciación"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 71773d69e6e98e7917f5e937f04cfa29197da7b8
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="depreciation-methods"></a>Métodos de depreciación
Hay ocho métodos de amortización disponibles:  
- Lineal  
- Regresivo 1  
- Regresivo 2  
- Rs1/L  
- Rs2/L  
- Definido por el usuario  
- Manual  

    Cuando utilice el método manual, debe introducir la amortización de forma manual en el diario general de activos fijos. El proceso **Calcular amortización** ignora los activos que utilizan el método de amortización manual. Puede utilizar este método para activos no sujetos a amortización, por ejemplo, los terrenos.  
- Convenio de medio año  

    Al utilizar este método, se amortiza el mismo importe de un activo fijo cada año.  

## <a name="straight-line-depreciation"></a>Amortización lineal
Al utilizar el método lineal, debe especificar una de las siguientes opciones en el libro de amortización de activos fijos:
- El periodo de amortización (años o meses) o una fecha final amortización  
- Un porcentaje fijo anual  
- Un importe fijo anual  
- Periodo de amortización  

### <a name="depreciation-period"></a>Periodo de amortización  
 Si introduce el periodo de amortización (número de años de amortización, número de meses o su fecha de finalización), el programa utiliza la siguiente fórmula para calcular el importe de amortización:  

*Importe amortización = ((Valor neto – Valor residual) x N. º días amortización) / Días restantes amortización*  

Los días restantes de amortización se calculan como el número de días de amortización, menos el número de días entre la fecha inicial de amortización y la última fecha de movimiento del activo fijo.  

El valor neto puede reducirse con apreciaciones, depreciaciones o importes especiales y provisiones registradas, según se desactive el campo **Incluye en cálc. amortización** y si se activa el campo **Parte valor neto** en la ventana **A/F Config. tipo registro**.  

Este cálculo garantiza que el activo fijo se amortice por completo al llegar la fecha final de amortización.    
### <a name="fixed-yearly-percentage"></a>Porcentaje fijo anual  
Si introdujo un porcentaje fijo anual, el programa utiliza la fórmula siguiente para calcular el importe de amortización:  

Importe amortización = (% Lineal x Base amortizable x N. º días amortización) / (100 x 360)  

### <a name="fixed-yearly-amount"></a>Importe fijo anual  
Si especificó un importe fijo anual, el sistema utiliza esta fórmula para calcular el importe de amortización:  

Importe amortización = (Importe fijo amortización x Número días amortización) / 360  

### <a name="example---straight-line-depreciation"></a>Ejemplo: amortización lineal
Un activo fijo tiene un costo de adquisición de $100 000. Su vida estimada es de ocho años.  

 El proceso **Calcular amortización** se realiza cada dos años. El movimiento de activos fijos es el siguiente:  

|Fecha|A/F Tipo registro|Días|Importe|Valor contable|  
|----------|---------------------|----------|------------|----------------|  
|01/01/10|Costo|*|100,000.00|100,000.00|  
|30/06/10|Amortización|180|-6,250.00|93,750.00|  
|31/12/10|Amortización|180|-6,250.00|87,500.00|  
|30/06/11|Amortización|180|-6,250.00|81,250.00|  
|31/12/11|Amortización|180|-6,250.00|75,000.00|  
|30/06/17|Amortización|180|-6,250.00|6,250.00|  
|31/12/17|Amortización|180|-6,250.00|0|  

* Fecha inicio amortización  

## <a name="declining-balance-1-depreciation"></a>Amortización con regresivo 1
Este es un método de amortización acelerado que coloca la mayor parte del costo de un activo en los primero años de su vida útil. Si utiliza este método, deberá introducir un porcentaje fijo anual.  

El programa utiliza la siguiente fórmula para calcular importes de amortización:  

*Importe amortización = (% Regresivo x Nº días amortización x Base amortizable / (100 x 360)*  

La base amortizable se calcula como el valor neto menos la amortización desde la fecha inicial del ejercicio actual.  

El importe de amortización registrado puede contener ciertos movimientos con diferentes tipos de registros (depreciación, personalizado1 y personalizado2) registrados desde el inicio del año fiscal actual. Estos tipos de registro se incluyen en el importe de amortización registrado, si los campos **Tipo amortización** y **Componente valor contable** están activados en la ventana **Config. tipo registro A/F**.  

### <a name="example---declining-balance-1-depreciation"></a>Ejemplo: amortización con regresivo 1
Un activo fijo tiene un costo de adquisición de $100 000. El valor del campo **% Regresivo** es 25. El proceso **Calcular amortización** se realiza cada dos años. Los movimientos de activos fijos son los siguientes  

|Fecha|A/F Tipo registro|Días|Importe|Valor contable|  
|----------|---------------------|----------|------------|----------------|  
|01/01/10|Costos|*|100,000.00|100,000.00|  
|30/06/10|Amortización|180|-12,500.00|87,500.00|  
|31/12/10|Amortización|180|-12,500.00|75,000.00|  
|30/06/11|Amortización|180|-9,375.00|65,625.00|  
|31/12/11|Amortización|180|-9,375.00|56,250.00|  
|30/06/12|Amortización|180|-7,031.25|49,218.75|  
|31/12/12|Amortización|180|-7,031.25|42,187.50|  
|30/06/13|Amortización|180|-5,273.44|36,914.06|  
|31/12/13|Amortización|180|-5,273.44|31,640.62|  
|30/06/14|Amortización|180|-3,955.08|27,685.54|  
|31/12/14|Amortización|180|-3,955.08|23,730.46|  

* Fecha inicio amortización  

 Método de cálculo:  

*1er año: 25% de 100.000 = 25.000 = 12.500 + 12.500*

*2º año: 25% de 75.000 = 18.750 = 9.375 + 9.375*

*3er año: 25% de 56.250 = 14.062,50 = 7.031,25 + 7.031,25*

El cálculo continúa hasta que el valor neto iguala al importe de redondeo final o al valor residual que ha introducido.   

## <a name="declining-balance-2-depreciation"></a>Amortización con regresivo 2
Los métodos Regresivo 1 y Regresivo 2 calculan el mismo importe total de amortización para cada año. Sin embargo, si ejecuta el proceso **Calcular amortización** más de una vez al año, el método Rs1 dará como resultado importes de amortización iguales para cada periodo de amortización. Por otra parte, el método Rs2 dará como resultado importes de amortización cada vez más reducidos en cada periodo.  

### <a name="example---declining-balance-2-depreciation"></a>Ejemplo: amortización con regresivo 2
Un activo fijo tiene un costo de adquisición de $100 000. El valor del campo **% Regresivo** es 25. El proceso **Calcular amortización** se realiza cada dos años. Los movimientos de activos fijos son los siguientes:  

|Fecha|A/F Tipo registro|Días|Importe|Valor contable|  
|----------|---------------------|----------|------------|----------------|  
|01/01/10|Costos|*|100,000.00|100,000.00|  
|30/06/10|Amortización|180|-13,397.46|86,602.54|  
|31/12/10|Amortización|180|-11,602.54|75,000.00|  
|30/06/11|Amortización|180|-10,048.09|64,951.91|  
|31/12/11|Amortización|180|-8,701.91|56,250.00|  

* Fecha inicio amortización  

Método de cálculo:
- VN = Valor neto  
- ND = Número días amortización  
- PR = porcentaje regresivo  
- P = PR/100  
- D = ND/360  

La formula para calcular los importes de amortización es:  

*IA = VN x (1-(1-P)<sup>D<sup>)*  

Los valores de amortización son:  

|Fecha|Cálculo|  
|----------|-----------------|  
|30/06/10|IA = 100.000 x (1 - (1 - 0,25)<sup>0,5<sup>) = 13.397,46|  
|31/12/10|IA = 86.602,54 x (1 - (1 - 0,25)<sup>0,5<sup>) = 11.602,54|  
|30/06/11|IA = 75.000 x (1 - (1 - 0,25)<sup>0,5<sup>) = 10.048,09|  
|31/12/11|IA = 64.951,91 x (1 - (1 - 0,25)<sup>0,5<sup>) = 8.701,91|  

## <a name="db1sl-depreciation"></a>Amortización Rs1/L
El cálculo continúa hasta que el valor neto iguala al importe de redondeo final o al valor residual que ha introducido.

Rs1/L es una combinación abreviada de Regresivo 1 y Lineal.  

El proceso **Calcular amortización** calcula un importe lineal y otro regresivo, pero sólo se transfiere al diario el mayor de los dos importes.  

El sistema puede manipular cálculos regresivos con varios porcentajes.  

Si utiliza este método, deberá introducir la vida útil estimada y el porcentaje regresivo en la ventana **A/F Libros amortización**.  

### <a name="example---db1-sl-depreciation"></a>Ejemplo: amortización Rs1/L
Un activo fijo tiene un costo de adquisición de $100 000. En la ventana **A/F Crear libros amortización**, el campo **% disminución de saldo** contiene 25 y el campo **N. º años amortización** contiene 8. El proceso **Calcular amortización** se realiza cada dos años.  

Los movimientos de activos fijos son los siguientes:  

|Fecha|A/F Tipo registro|Días|Importe|Valor contable|  
|----------|---------------------|----------|------------|----------------|  
|01/01/10|Costos|*|100,000.00|100,000.00|  
|30/06/10|Amortización|180|-12,500.00|87,500.00|  
|31/12/10|Amortización|180|-12,500.00|75,000.00|  
|30/06/11|Amortización|180|-9,375.00|65,625.00|  
|31/12/11|Amortización|180|-9,375.00|56,250.00|  
|30/06/12|Amortización|180|-7,031.25|49,218.75|  
|31/12/12|Amortización|180|-7,031.25|42,187.50|  
|30/06/13|Amortización|180|-5,273.44|36,914.06|  
|31/12/13|Amortización|180|-5,273.44|31,640.62|  
|30/06/14|Amortización|180|-3,955.08|27,685.54|  
|31/12/14|Amortización|180|-3,955.08|23,730.46|  
|30/06/15|Amortización|180|-3,955.08|19.775,38 L|  
|31/12/15|Amortización|180|-3,955.08|15.820,30 L|  
|30/06/16|Amortización|180|-3,955.08|11.865,22 L|  
|31/12/16|Amortización|180|-3,955.07|7.910,15 L|  
|30/06/17|Amortización|180|-3,955.08|3.955,07 L|  
|31/12/17|Amortización|180|-3,955.07|0,00 L|  

* Fecha inicio amortización  

"L" después del valor neto significa que se utilizó el método lineal.  

Método de cálculo:  

1er año:

*Importe regresivo: 25% de 100.000 = 25.000=12.500+12.500*  

*Importe lineal = 100.000/8=12.500=6.250+6.250*  

Se utiliza el importe regresivo, ya que es el importe mayor.  

6º año (2015):  

*Importe regresivo: 25% de 23,730.46 = 4,943.85=2,471.92+2,471.92*  

*Importe lineal = 23.730,46/3 = 7.910,15 = 3.995,07 + 3.995,08*  

Se utiliza el importe lineal, ya que es el importe mayor.  

## <a name="user-defined-depreciation"></a>Amortización definida por el usuario
El sistema dispone de una utilidad que permite configurar los métodos de amortización definidos por el usuario.  

Con un método definido por el usuario, se utiliza la ventana **Tablas amortización**, donde debe introducir un porcentaje de amortización para cada periodo (mes, trimestre, año o periodo contable).  

La formula para calcular los importes de amortización es:  

Importe amortización = (% Amortización x N. º días amortización x Base amortizable / (100 x 360)

### <a name="depreciation-based-on-number-of-units"></a>Amortización según el número de unidades  
 Este método definido por el usuario también se puede utilizar para amortizar según el número de unidades, por ejemplo, en el caso de máquinas de producción con una capacidad de vida establecida. En la ventana **Tablas amortización**, puede introducir el número de unidades que pueden producirse en cada periodo (mes, trimestre, año o periodo contable).  

### <a name="to-set-up-user-defined-depreciation-methods"></a>Para configurar métodos de amortización definidos por usuario
En la ventana **Tabla amortización**, puede configurar métodos de amortización definidos por el usuario. Por ejemplo, puede configurar la amortización según el número de unidades.  

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Tablas amortización** y, a continuación, seleccione el vínculo relacionado.
2. En la ventana **Lista tablas amortización**, elija la acción **Nuevo**.
3. En la ventana **Ficha tablas amortización**, rellene los campos según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.

### <a name="example---user-defined-depreciation"></a>Ejemplo: amortización definida por el usuario
Por motivos de impuestos puede utilizar un método amortización que le permita amortizar activos de forma acelerada.  

Por tanto, podría utilizar las siguientes tasas de depreciación para un activo fijo con una duración de tres años para fines fiscales:  

año 1: 25%  

año 2: 38%  

año 3: 37%  

El costo es de 100.000 $ y el periodo de amortización es de cinco años. La amortización se calcula anualmente.  

|Fecha|A/F Tipo registro|Días|Importe|Valor contable|  
|----------|---------------------|----------|------------|----------------|  
|01/01/10|Costo|*|100,000.00|100,000.00|  
|31/12/10|Amortización|360|-25,000.00|75,000.00|  
|31/12/11|Amortización|360|-38,000.00|37,000.00|  
|31/12/12|Amortización|360|-37,000.00|0|  
|31/12/13|Amortización|Ninguno|Ninguno|0|  
|31/12/14|Amortización|Ninguno|Ninguno|0|  

* Fecha inicio amortización  

Si utiliza un método definido por el usuario, los campos **1ª fecha amort. def.-usuario** y **Fecha inicio amortización** deben rellenarse en la ventana **A/F Libros amortización**. El campo **1ª fecha amort. def.-usuario** y el contenido del campo **Longitud periodo** de la ventana **Tablas amortización** se utilizan para determinar los intervalos de tiempo a utilizar en los cálculos de amortización. Así se garantiza que el sistema comenzará a utilizar el porcentaje especificado para todos los activos en el mismo día. El campo **Fecha inicio amortización** se utiliza para calcular el número de días de amortización.  

En el ejemplo anterior, los campos **1ª fecha amort. def.-usuario** y **Fecha inicio amortización** contienen 01/01/01. Sin embargo, si el campo **1ª fecha amort. def.-usuario** tuviera 01/01/10 y el campo **Fecha inicio amortización** tuviera 01/04/11, el resultado podría ser:  

|Fecha|A/F Tipo registro|Días|Importe|Valor contable|  
|----------|---------------------|----------|------------|----------------|  
|01/01/10|Costo|*|100,000.00|100,000.00|  
|31/12/10|Amortización|270|-18,750.00|81,250.00|  
|31/12/11|Amortización|360|-38,000.00|42,250.00|  
|31/12/12|Amortización|360|-37,000.00|6,250.00|  
|31/12/13|Amortización|90|-6,250.00|0|  
|31/12/14|Amortización|Ninguno|Ninguno|0|  

* Fecha inicio amortización

## <a name="half-year-convention-depreciation"></a>Amortización de convenio de medio año   
El método Convenio medio año solo se aplicará si activó el campo **Usar convenio medio año** en la ventana fija **A/F Libro amortización**.  

Este método de amortización puede utilizarse junto con los siguientes métodos de amortización:  
- Lineal
- Regresivo 1
- Rs1/L  

Al aplicar el Convenio medio año, un activo tendrá seis meses de depreciación en el primer ejercicio, independientemente del contenido del campo **Fecha primera depreciación**.  

**Nota**. La vida estimada del activo fijo que resta después del primer ejercicio siempre será de medio año con el método Convenio de medio año. De esta manera, para poder aplicar correctamente el método Convenio medio año, el campo **Fecha final amortización** de la ventana **Libro de amortización activos** siempre debe contener una fecha exactamente seis meses antes de la fecha final del año fiscal en el que se amortizó totalmente el activo.  

### <a name="example---half-year-convention-depreciation"></a>Ejemplo - Amortización de convenio de medio año
Un activo fijo tiene un costo de adquisición de $100 000. La **Fecha inicio amortización** es 01/03/10. La vida estimada es de cinco años, por lo que la **Fecha final amortización** debe ser 30/06/15. El proceso **Calcular amortización** se realiza cada año. Este ejemplo sigue el calendario fiscal anual.  

 Los movimientos de activos fijos son los siguientes:  

|Fecha|A/F Tipo registro|Días|Importe|Valor contable|  
|----------|---------------------|----------|------------|----------------|  
|01/03/10|Costo|*|100,000.00|100,000.00|  
|31/12/10|Amortización|270|-10.000,00|90,000.00|  
|31/12/11|Amortización|360|-20.000,00|70,000.00|  
|31/12/12|Amortización|360|-20.000,00|50,000.00|  
|31/12/13|Amortización|360|-20.000,00|30,000.00|  
|31/12/14|Amortización|360|-20.000,00|10,000.00|  
|31/12/15|Amortización|180|-10.000,00|0.00|  

* Fecha inicio amortización  

## <a name="example---db1sl-depreciation-using-half-year-convention"></a>Ejemplo - Amortización Rs1/L utilizando el convenio de medio año  
Un activo fijo tiene un costo de adquisición de $100 000. La **Fecha inicio amortización** es 01/11/10. La vida estimada es de cinco años, por lo que la **Fecha final amortización** debe ser 30/06/15. En la ventana **A/F Libros amortización**, el campo **% disminución de saldo** contiene 40. El proceso **Calcular amortización** se realiza cada año. Este ejemplo sigue el calendario fiscal anual.  

Los movimientos de activos fijos son los siguientes:  

|Fecha|A/F Tipo registro|Días|Importe|Valor contable|  
|----------|---------------------|----------|------------|----------------|  
|01/11/10|Costo|*|100,000.00|100,000.00|  
|31/12/10|Amortización|60|-20.000,00|80,000.00|  
|31/12/11|Amortización|360|-32.000,00|48,000.00|  
|31/12/12|Amortización|360|-19.200,00|28,800.00|  
|31/12/13|Amortización|360|-11.520,00|17,280.00|  
|31/12/14|Amortización|360|-11.520,00|5.760,00 L|  
|31/12/15|Amortización|180|  -5.760,00|0,00 L|  

 * Fecha inicio amortización  

"L" después del valor neto significa que se utilizó el método lineal.  

Método de cálculo:  

1er año:  

*Importe regresivo = Importe todo el año = 40% de 100.000 = 40.000, por lo que por medio año, 40.000/ 2 = 20.000*  

*Importe lineal = Importe todo el año = 100.000 / 5 = 20.000, por lo que por medio año = 20.000 / 2 = 10.000*  

Se utiliza el importe regresivo, ya que es el importe mayor.  

5º año (2004):  

*Importe regresivo: 40% de 17.280,00 = 6.912,00*  

*Importe lineal = 28.800 / 1,5 = 11.520,00*  

Se utiliza el importe lineal, ya que es el importe mayor.

## <a name="duplicating-entries-to-more-depreciation-books"></a>Duplicación de movimientos en más libros de amortización
Si tiene tres libros de amortización, B1, B2 y B3, y desea duplicar los movimientos del B1 al B2 y B3, puede activar el campo **Compone lista duplicados** en las fichas del libro de amortización para B2 y B3. Esto puede resultar de utilidad si el libro de amortización B1 está integrado en la contabilidad y utiliza el diario general de activos fijos, y los libros de amortización B2 y B3 no están integrados con la contabilidad y utiliza el diario de activos.  

Cuando introduzca un movimiento en B1 del diario general de activos fijos y active el campo **Utiliza lista duplicados**, el programa duplicará el movimiento en los libros B2 y B3 del diario de activos en el momento de registrar el movimiento.  

**Nota**: No es posible duplicar en el mismo diario y proceso de diario desde el que está duplicando. Si registra movimientos en el diario general de activos fijos, podrá duplicarlos en el diario de activos o en el diario general de activos fijos mediante otro proceso.  

**Nota**: No es posible utilizar el mismo número de serie en los diarios generales de activos fijos y en los diarios de activos fijos. Al registrar movimientos en los diarios generales de activos fijos, debe dejar en blanco el campo **N. º documento**. campo vacío. Si introduce un número en el campo, el programa duplicará el número en el diario de activos fijos y no podrá registrar el diario a menos que cambie el número de documento manualmente.     

## <a name="see-also"></a>Consulte también
[Gestión de activos fijos](fa-manage.md)  
[Configuración de activos fijos](fa-setup.md)  
[Finanzas](finance-setup.md)  
[Este es Dynamics NAV](across-get-started.md)
