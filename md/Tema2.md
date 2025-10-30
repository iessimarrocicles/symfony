# 🧩 TEMA 2: El patró MVC en Symfony

## 1️⃣ Què és el patró MVC?

**MVC** són les sigles de **Model - Vista - Controlador**, i és el patró d’arquitectura més utilitzat en el desenvolupament web.

L’objectiu és **separar les responsabilitats** del codi per a aconseguir aplicacions més netes, modulars i fàcils de mantenir.

| Component | Descripció | Exemple |
|------------|-------------|----------|
| **Model** | Gestiona les dades i la lògica de negoci. Representa la informació que utilitza l’aplicació. | Entitats de Doctrine com `Contacte`, `Usuari`, `Llibre`... |
| **Vista** | S’encarrega de mostrar la informació a l’usuari (interfície HTML). | Fitxers `.html.twig` dins la carpeta `templates/` |
| **Controlador** | Gestiona les peticions de l’usuari, interactua amb el model i tria quina vista mostrar. | Classes dins `src/Controller/` |

### 🟢 Avantatges del patró MVC
- Codi **més estructurat i mantenible**.  
- Facilita el **treball en equip** (programador ↔ dissenyador).  
- Permet **reutilitzar** components i millorar la seguretat.  

---

## 2️⃣ Controladors i rutes en Symfony

Per a crear una pàgina en Symfony calen **dos elements principals**:

1. **Una ruta** → defineix l’URL que activarà el controlador.  
2. **Un controlador** → és la classe que conté el codi que es vol executar.

---

### 🔹 Exemple bàsic

Fitxer: `src/Controller/IniciController.php`

```php
<?php
namespace App\Controller;

use Symfony\Component\HttpFoundation\Response;
use Symfony\Component\Routing\Annotation\Route;

class IniciController
{
    #[Route('/', name: 'inici')]
    public function inici(): Response
    {
        return new Response('Benvingut/da al web de contactes');
    }
}
