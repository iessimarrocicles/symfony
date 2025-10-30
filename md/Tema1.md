---
title: "TEMA 1 — Introducció als frameworks PHP i a Symfony"
icon: material/language-php
nav:
  - TEMA 1: 'tema01-introduccio.md'
---

# 🧩 TEMA 1 — Introducció als frameworks PHP i a Symfony

## 1. Què és un framework?

Un **framework** és una eina que proporciona un conjunt d’elements i regles per a facilitar el **desenvolupament d’aplicacions web**.  
En el cas dels **frameworks PHP**, ofereixen:

- Una **estructura de treball** predefinida (normalment basada en el patró **MVC**).  
- Eines per a crear i gestionar **models de dades**, **controladors** i **vistes**.  
- Suport per a **rutes**, **injecció de dependències**, **seguretat** i **testejos automàtics**.  

Això permet que el codi siga més **organitzat**, **modular** i **fàcil de mantindre**.

---

## 2. Exemples de frameworks PHP

Actualment hi ha molts frameworks PHP disponibles. A continuació tens una comparativa dels més coneguts:

| Framework | Any | Característiques principals |
|------------|-----|-----------------------------|
| **Laravel** | 2011 | Elegant, simple i amb gran comunitat. Ideal per a projectes nous. |
| **Symfony** | 2005 | Molt estructurat, modular i estable. Segueix bones pràctiques de programació. |
| **CodeIgniter** | 2006 | Lleuger i ràpid d’aprendre, però més limitat. |
| **Phalcon** | 2012 | Extremadament ràpid i flexible, pot funcionar com a microframework. |
| **CakePHP** | 2005 | Senzill i amb una comunitat àmplia. |
| **Zend** | 2006 | Robust i orientat a empreses, encara que menys utilitzat hui dia. |

➡️ Tots ells segueixen el patró **MVC** i permeten el desenvolupament tant de webs completes com de **serveis RESTful**.

---

## 3. Quin triar?

Depén de les necessitats del projecte i de l’experiència de l’equip:

- **Projectes senzills o d’aprenentatge:** *CodeIgniter* o *CakePHP*.  
- **Projectes professionals o de llarga duració:** *Symfony* o *Laravel*.  

> 🧠 Symfony és més complex al principi, però proporciona una base sòlida i escalable.

---

## 4. Per què triar Symfony?

Symfony és un framework **modern, segur i molt complet**. Els seus principals avantatges són:

- 🧱 **Estructura robusta i modular.**  
- 🕓 **Versions LTS** (Long Term Support) amb manteniment garantit.  
- 🌍 **Gran comunitat** i **documentació oficial** excel·lent.  
- 💡 **Bones pràctiques integrades**, seguint estàndards PSR.  
- 🔌 **Integració amb llibreries de tercers** com:
  - **Twig** → motor de plantilles per a generar vistes.
  - **Doctrine** → ORM per a treballar amb bases de dades com a objectes.

---

## 5. Recursos necessaris

Per treballar amb **Symfony 6.1** o superior, cal tindre instal·lats els següents components:

| Component | Descripció |
|------------|-------------|
| **Servidor web** | Apache o Nginx amb suport per a PHP 8.1+ |
| **Base de dades** | MariaDB o MySQL |
| **PHP** | Versió 8.1 o posterior |
| **Composer** | Gestor de dependències per a PHP |
| **Symfony CLI** | Eina oficial per a crear i gestionar projectes |
| **IDE / Editor** | VS Code, PHPStorm o qualsevol altre amb suport per a PHP |
| **Sistema operatiu** | Ubuntu 22.04 (recomanat) o Windows amb WSL2 |

---

## 6. Instal·lació bàsica (resum)

Per crear un nou projecte Symfony amb l’esquelet complet:

```bash
composer create-project symfony/website-skeleton nom_projecte
```

O per crear un projecte lleuger, sense bundles innecessaris:

```bash
composer create-project symfony/skeleton nom_projecte
```

Després pots iniciar el servidor intern de Symfony amb:

```bash
symfony serve
```

---

## 7. Conclusió

Symfony és una de les millors opcions per a aprendre **desenvolupament web en entorn servidor** amb PHP.  
Et permet entendre com funciona el **patró MVC**, treballar amb **bones pràctiques** i construir aplicacions **professionals, segures i escalables**.

> 💬 En resum: Symfony és exigent al principi, però t’ensenya a programar “bé”.

---

**Referències:**
- [Documentació oficial de Symfony](https://symfony.com/doc/current/index.html)
- [Releases Symfony](https://symfony.com/releases)

