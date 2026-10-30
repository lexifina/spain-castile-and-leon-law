# Castile and León: law history in git

The law of the autonomous community of Castile and León (Comunidad de Castilla y León, Spain) as a git history: one file per article, one commit per norm that changed it, dated the day the change took effect, with the amending norm as the commit's author. `git blame` names the norm behind every paragraph; `git log` lists every change to an article; checking out a date gives the text in force that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `es-cl/`. Spain's national law is in [lexifina/spain-law](https://github.com/lexifina/spain-law).

The text is in Spanish, exactly as the BOE's consolidated text prints it. Texts in co-official languages are not included.

Basado en datos de la Agencia Estatal Boletín Oficial del Estado (<https://www.boe.es>). Every text here is a consolidated text for information only (texto consolidado de carácter meramente informativo), not an official publication.

## What this repository holds

196 norms with 731 versions so far: the Estatuto de Autonomía first, then the laws, decree-laws and legislative decrees in force that the BOE consolidates, oldest first, added in parts of about 50. 8 of them are repealed norms the BOE consolidates: their whole history is kept, and their last commit removes the text on the day the repeal took effect, credited to the repealing norm. Regulations are not included (the BOE consolidates no autonomic decrees or orders).

| Folder | Norm | Versions | History | BOE last updated |
| --- | --- | ---: | --- | --- |
| `estatuto-de-autonomia/` | Ley Orgánica 14/2007, de 30 de noviembre, de reforma del Estatuto de Autonomía de Castilla y León. | 3 | as first published, then each change: 1 December 2007 to 11 April 2011 | 2026-01-20 |
| `ley-1986-001/` | Ley 1/1986, de 31 de marzo, de creación de la Reserva Nacional de Caza de "Las Lagunas de Villafáfila". | 1 | as first published: 10 April 1986 | 2025-12-17 |
| `ley-1987-003/` | Ley 3/1987, de 30 de marzo, Electoral de Castilla y León. | 5 | as first published, then each change: 2 April 1987 to 7 July 2017 | 2026-04-15 |
| `ley-1987-007/` | Ley 7/1987, de 8 de mayo, por la que se regula el procedimiento de designación de Senadores representantes de la Comunidad de Castilla y León. | 3 | as first published, then each change: 12 May 1987 to 15 November 2022 | 2025-12-17 |
| `ley-1987-013/` | Ley 13/1987, de 29 de diciembre, por la que se determina la sede de las Instituciones de Autogobierno de Castilla y León. | 1 | as first published: 12 January 1988 | 2025-12-17 |
| `ley-1987-014/` | Ley 14/1987, de 29 de diciembre, por la que se determina la sede del Tribunal Superior de Justicia de Castilla y León. | 1 | as first published: 12 January 1988 | 2025-12-17 |
| `ley-1989-003/` | Ley 3/1989, de 13 de abril, por la que se determina la capitalidad de los partidos judiciales en la Comunidad de Castilla y León. | 1 | as first published: 11 May 1989 | 2025-12-17 |
| `ley-1989-005/` | Ley 5/1989, de 27 de junio, por la que se declara el parque de las Hoces del río Duratón. | 2 | oldest version available, then each change: 11 July 1989 to 30 May 1991 | 2025-12-17 |
| `ley-1989-009/` | Ley 9/1989, de 30 de noviembre, de Bibliotecas de Castilla y León. | 3 | as first published, then each change: 11 January 1990 to 7 July 2017 | 2025-12-17 |
| `ley-1990-005/` | Ley 5/1990, de 17 de mayo, por la que se crea la Orquesta Sinfónica de Castilla y León, Sociedad Anónima. | 1 | as first published: 30 May 1990 | 2026-04-22 |
| `ley-1990-013/` | Ley 13/1990, de 28 de noviembre, del Consejo Económico y Social. | 5 | oldest version available, then each change: 15 December 1990 to 4 July 2013 | 2026-10-20 |
| `ley-1991-001/` | Ley 1/1991, de 14 de marzo, por la que se crea y regula la Comarca de El Bierzo. | 2 | oldest version available, then each change: 9 April 1991 to 22 December 2010 | 2025-12-17 |
| `ley-1991-006/` | Ley 6/1991, de 19 de abril, de Archivos y del Patrimonio Documental de Castilla y León. | 6 | as first published, then each change: 4 June 1991 to 7 July 2017 | 2025-12-17 |
| `ley-1991-007/` | Ley 7/1991, de 30 de abril, por la que se regula el Fondo de Compensación Regional. | 2 | oldest version available, then each change: 17 June 1991 to 12 June 1992 | 2025-12-17 |
| `ley-1994-002/` | Ley 2/1994, de 9 de marzo, del Procurador del Común de Castilla y León. | 3 | as first published, then each change: 17 March 1994 to 4 July 2013 | 2025-12-17 |
| `ley-1994-003/` | Ley 3/1994, de 29 de marzo, de Prevención, Asistencia e Integración Social de Drogodependientes de Castilla y León. | 6 | as first published, then each change: 7 April 1994 to 20 September 2014 | 2025-12-17 |
| `ley-1994-006/` | Ley 6/1994, de 19 de mayo, de Sanidad Animal de Castilla y León. | 6 | as first published, then each change: 16 June 1994 to 14 July 2024 | 2025-12-17 |
| `ley-1994-012/` | Ley 12/1994, de 18 de julio, de Declaración del Parque Regional de Picos de Europa, en Castilla y León. | 3 | oldest version available, then each change: 17 August 1994 to 10 January 2021 | 2025-12-17 |
| `ley-1995-001/` | Ley 1/1995, de 6 de abril, de Cámaras Agrarias de Castilla y León. | 6 | as first published, then each change: 5 September 1996 to 15 May 2024 | 2025-12-18 |
| `ley-1995-002/` | Ley 2/1995, de 6 de abril, por la que se crea la Gerencia de Servicios Sociales de Castilla y León. | 6 | as first published, then each change: 1 August 1995 to 1 January 2014 | 2025-12-18 |
| `ley-1996-001/` | Ley 1/1996, de 27 de marzo, reguladora de la cuestión de confianza y de la facultad del Presidente de la Junta de disolución de las Cortes de Castilla y León. | 1 | oldest version available: 10 April 1996 | 2023-12-26 |
| `ley-1996-003/` | Ley 3/1996, de 20 de junio, de Declaración de Parque Regional de la Sierra de Gredos. | 1 | oldest version available: 18 July 1996 | 2025-12-18 |
| `ley-1996-007/` | Ley 7/1996, de 3 de diciembre, de Creación del Ente Público Regional de la Energía de Castilla y León. | 5 | as first published, then each change: 10 December 1996 to 25 June 2022 | 2025-12-18 |
| `ley-1996-008/` | Ley 8/1996, de 27 de diciembre, de Medidas Financieras, Presupuestarias y Económicas. | 2 | as first published, then each change: 1 January 1997 to 1 March 2012 | 2025-12-18 |
| `ley-1997-004/` | Ley 4/1997, de 24 de abril, por la que se reconoce como Universidad privada a la Universidad S.E.K., con sede en Segovia. | 2 | as first published, then each change: 1 May 1997 to 27 December 2008 | 2025-12-18 |
| `ley-1997-005/` | Ley 5/1997, de 24 de abril, de protección de los animales de compañía. | 4 | as first published, then each change: 30 July 1997 to 7 July 2017 | 2025-12-18 |
| `ley-1997-006/` | Ley 6/1997, de 22 de mayo, de Ferias Comerciales Oficiales de Castilla y León. | 2 | as first published, then each change: 4 June 1997 to 27 December 2009 | 2025-12-18 |
| `ley-1997-007/` | Ley 7/1997, de 17 de junio, de Declaración de la Reserva Natural del Valle de Iruelas (Ávila). | 1 | as first published: 14 July 1997 | 2025-12-18 |
| `ley-1997-008/` | Ley 8/1997, de 8 de julio, de Colegios Profesionales de Castilla y León. | 3 | oldest version available, then each change: 30 July 1997 to 11 December 2015 | 2025-12-18 |
| `ley-1998-001/` | Ley 1/1998, de 4 de junio, de Régimen Local de Castilla y León. | 8 | as first published, then each change: 12 June 1998 to 15 May 2024 | 2025-12-18 |
| `ley-1998-003/` | Ley 3/1998, de 24 de junio, de accesibilidad y supresión de barreras. | 4 | as first published, then each change: 1 October 1998 to 8 October 2019 | 2025-12-18 |
| `ley-1998-004/` | Ley 4/1998, de 24 de junio, reguladora del Juego y de las Apuestas de Castilla y León. | 14 | as first published, then each change: 2 July 1998 to 21 April 2024 | 2025-12-18 |
| `ley-1998-010/` | Ley 10/1998, de 5 de diciembre, de Ordenación del Territorio de la Comunidad de Castilla y León. | 11 | as first published, then each change: 11 December 1998 to 15 May 2024 | 2025-12-18 |
| `ley-1998-012/` | Ley 12/1998, de 5 de diciembre, de Creación del Consejo de Colegios Profesionales de Diplomados de Enfermería de Castilla y León. | 1 | as first published: 11 December 1998 | 2025-12-18 |
| `ley-1999-005/` | Ley 5/1999, de 8 de abril, de Urbanismo de Castilla y León. | 21 | as first published, then each change: 5 May 1999 to 5 December 2025 | 2026-03-04 |
| `ley-2000-002/` | Ley 2/2000, de 10 de mayo, de creación del Colegio Profesional de Podólogos de Castilla y León. | 1 | as first published: 20 May 2000 | 2025-12-18 |
| `ley-2000-003/` | Ley 3/2000, de 10 de mayo, de creación del Consejo de Colegios Profesionales de Farmacéuticos de Castilla y León. | 1 | as first published: 20 May 2000 | 2025-12-18 |
| `ley-2000-004/` | Ley 4/2000, de 27 de junio, de declaración del Parque Natural de Fuentes Carrionas y Fuente Cobre-Montaña Palentina (Palencia). | 4 | as first published, then each change: 6 July 2000 to 10 January 2021 | 2025-12-18 |
| `ley-2000-005/` | Ley 5/2000, de 27 de junio, de creación del Colegio Profesional de Protésicos Dentales de Castilla y León. | 1 | as first published: 6 July 2000 | 2025-12-18 |
| `ley-2000-006/` | Ley 6/2000, de 27 de junio, de creación del Colegio Profesional de Fisioterapeutas de Castilla y León. | 1 | as first published: 6 July 2000 | 2025-12-18 |
| `ley-2000-007/` | Ley 7/2000, de 11 de julio, de Estadística de Castilla y León. | 1 | as first published: 8 August 2000 | 2025-12-18 |
| `ley-2000-008/` | Ley 8/2000, de 11 de julio, de Declaración del Parque Natural de Las Batuecas-Sierra de Francia (Salamanca). | 2 | as first published, then each change: 20 July 2000 to 27 December 2008 | 2025-12-18 |
| `ley-2000-009/` | Ley 9/2000, de 11 de julio, de Declaración de la Reserva Natural del Sabinar de Calatañazor (Soria). | 1 | as first published: 20 July 2000 | 2025-12-18 |
| `ley-2001-003/` | Ley 3/2001, de 3 de julio, del Gobierno y de la Administración de la Comunidad de Castilla y León. | 12 | as first published, then each change: 26 July 2001 to 15 May 2024 | 2025-12-18 |
| `ley-2001-004/` | Ley 4/2001, de 4 de julio, reguladora de la Iniciativa Legislativa Popular y de los Ayuntamientos de Castilla y León. | 3 | as first published, then each change: 10 July 2001 to 14 January 2017 | 2025-12-18 |
| `ley-2001-006/` | Ley 6/2001, de 22 de noviembre, de Creación del Consejo de Colegios Profesionales de Peritos e Ingenieros Técnicos Industriales de Castilla y León. | 1 | as first published: 29 November 2001 | 2025-12-18 |
| `ley-2001-007/` | Ley 7/2001, de 22 de noviembre, de Creación del Consejo de Colegios Profesionales de Veterinarios de Castilla y León. | 1 | as first published: 29 November 2001 | 2025-12-18 |
| `ley-2001-008/` | Ley 8/2001, de 22 de noviembre, de Creación del Consejo de Colegios Profesionales de Médicos de Castilla y León. | 1 | as first published: 29 November 2001 | 2025-12-18 |
| `ley-2001-009/` | Ley 9/2001, de 22 de noviembre, de Creación del Consejo de Colegios Profesionales de Diplomados en Trabajo Social y Asistentes Sociales de Castilla y León. | 1 | as first published: 29 November 2001 | 2025-12-18 |
| `ley-2001-010/` | Ley 10/2001, de 22 de noviembre, de Creación del Consejo de Colegios Profesionales de Mediadores de Seguros Titulados de Castilla y León. | 1 | as first published: 29 November 2001 | 2025-12-18 |
| `ley-2001-012/` | Ley 12/2001, de 20 de diciembre, de Tasas y Precios Públicos de la Comunidad de Castilla y León. | 23 | as first published, then each change: 27 January 2001 to 15 May 2024 | 2026-01-02 |
| `ley-2001-013/` | Ley 13/2001, de 20 de diciembre, de Ordenación Farmacéutica de la Comunidad de Castilla y León. | 7 | oldest version available, then each change: 15 January 2002 to 20 January 2026 | 2026-01-20 |
| `ley-2002-001/` | Ley 1/2002, de 9 de abril, reguladora del Consejo Consultivo de Castilla y León. | 6 | as first published, then each change: 12 May 2002 to 20 September 2014 | 2025-12-18 |
| `ley-2002-002/` | Ley 2/2002, de 9 de abril, reguladora del Consejo de Cuentas de Castilla y León. | 4 | as first published, then each change: 7 May 2002 to 4 July 2013 | 2025-12-18 |
| `ley-2002-003/` | Ley 3/2002, de 9 de abril, de Educación de Personas Adultas de Castilla y León. | 1 | as first published: 23 April 2002 | 2025-12-18 |
| `ley-2002-005/` | Ley 5/2002, de 11 de abril, de declaración del Parque Natural de Arribes del Duero (Salamanca-Zamora). | 1 | as first published: 27 April 2002 | 2025-12-18 |
| `ley-2002-006/` | Ley 6/2002, de 11 de abril, de declaración de la Reserva Natural de Riberas de "Castronuño-Vega del Duero" (Valladolid). | 1 | as first published: 27 April 2002 | 2025-12-18 |
| `ley-2002-004/` | Ley 4/2002, de 11 de abril, de Cooperativas de la Comunidad de Castilla y León. | 5 | as first published, then each change: 16 May 2002 to 15 July 2018 | 2025-12-18 |
| `ley-2002-007/` | Ley 7/2002, de 3 de mayo, de creación del Instituto Tecnológico Agrario de Castilla y León. | 9 | as first published, then each change: 9 May 2002 to 7 March 2023 | 2025-12-18 |
| `ley-2002-008/` | Ley 8/2002, de 18 de junio, por la que se reconoce como Universidad Privada a la "Universidad Europea Miguel de Cervantes", con sede en Valladolid. | 1 | as first published: 25 June 2002 | 2025-12-18 |
| `ley-2002-009/` | Ley 9/2002, de 10 de julio, para la declaración de proyectos regionales de infraestructuras de residuos de singular interés para la Comunidad. | 2 | as first published, then each change: 13 July 2002 to 2 July 2013 | 2025-12-18 |
| `ley-2002-011/` | Ley 11/2002, de 10 de julio, de Juventud de Castilla y León. | 7 | oldest version available, then each change: 19 September 2002 to 19 October 2021 | 2025-12-18 |
| `ley-2002-013/` | Ley 13/2002, de 15 de julio, de Fundaciones de Castilla y León. | 6 | as first published, then each change: 8 August 2002 to 15 May 2024 | 2025-12-18 |
| `ley-2002-014/` | Ley 14/2002, de 25 de julio, de Promoción, Atención y Protección a la Infancia en Castilla y León. | 2 | as first published, then each change: 18 August 2002 to 20 September 2014 | 2025-12-18 |
| `ley-2002-017/` | Ley 17/2002, de 19 de diciembre, de Fomento y Coordinación General de la Investigación Científica, Desarrollo e Innovación Tecnológica (I + D + I) en Castilla y León. | 2 | as first published, then each change: 25 December 2002 to 20 September 2014 | 2025-12-18 |
| `ley-2002-018/` | Ley 18/2002, de 19 de diciembre, de creación del Consejo de Colegios Profesionales de Abogados de Castilla y León. | 1 | as first published: 25 December 2002 | 2025-12-18 |
| `ley-2002-019/` | Ley 19/2002, de 19 de diciembre, de Creación del Consejo de Colegios Profesionales de Procuradores de los Tribunales de Castilla y León. | 1 | as first published: 25 December 2002 | 2025-12-18 |
| `ley-2002-020/` | Ley 20/2002, de 19 de diciembre, de Creación del Consejo de Colegios Profesionales de Aparejadores y Arquitectos Técnicos de Castilla y León. | 1 | as first published: 25 December 2002 | 2025-12-18 |
| `ley-2003-001/` | Ley 1/2003, de 3 de marzo, de Igualdad de oportunidades entre mujeres y hombres en Castilla y León. | 4 | as first published, then each change: 27 March 2003 to 20 September 2014 | 2025-12-18 |
| `ley-2003-003/` | Ley 3/2003, de 28 de marzo, de Universidades de Castilla y León. | 4 | as first published, then each change: 5 April 2003 to 7 July 2017 | 2026-03-19 |
| `ley-2003-004/` | Ley 4/2003, de 28 de marzo, de creación del Colegio Profesional de Ingenieros en Informática de Castilla y León. | 1 | as first published: 5 April 2003 | 2025-12-18 |
| `ley-2003-005/` | Ley 5/2003, de 3 de abril, de atención y protección a las personas mayores de Castilla y León. | 3 | oldest version available, then each change: 28 April 2003 to 20 September 2014 | 2025-12-18 |
| `ley-2003-006/` | Ley 6/2003, de 3 de abril, reguladora de la asistencia jurídica a la Comunidad de Castilla y León. | 3 | as first published, then each change: 28 April 2003 to 17 March 2021 | 2025-12-18 |
| `ley-2003-008/` | Ley 8/2003, de 8 de abril, sobre derechos y deberes de las personas en relación con la salud. | 1 | as first published: 14 May 2003 | 2025-12-18 |
| `ley-2003-009/` | Ley 9/2003, de 8 de abril, de Coordinación de Policías Locales de Castilla y León. | 6 | as first published, then each change: 4 May 2003 to 15 May 2024 | 2026-04-22 |
| `ley-2003-010/` | Ley 10/2003, de 8 de abril, de creación del servicio público de empleo de Castilla y León. | 4 | as first published, then each change: 15 April 2003 to 20 September 2014 | 2025-12-18 |
| `ley-2004-001/` | Ley 1/2004, de 13 de octubre, de Creación del Consejo de Colegios Profesionales de Agentes Comerciales de Castilla y León. | 1 | as first published: 21 October 2004 | 2025-12-18 |
| `ley-2004-002/` | Ley 2/2004, de 13 de octubre, de Creación del Consejo de Colegios Profesionales de Doctores y Licenciados en Filosofía y Letras y en Ciencias de Castilla y León. | 1 | as first published: 21 October 2004 | 2025-12-18 |
| `ley-2004-003/` | Ley 3/2004, de 13 de octubre, de Creación del Consejo de Colegios Profesionales de Agentes de la Propiedad Inmobiliaria de Castilla y León. | 1 | as first published: 21 October 2004 | 2025-12-18 |
| `ley-2004-004/` | Ley 4/2004, de 13 de octubre, de Creación del Consejo de Colegios Profesionales de Secretarios, Interventores y Tesoreros de la Administración Local de Castilla y León. | 1 | as first published: 21 October 2004 | 2025-12-18 |
| `ley-2004-005/` | Ley 5/2004, de 21 de diciembre, de declaración del Parque Natural de Hoces del Río Riaza (Segovia). | 1 | as first published: 23 December 2004 | 2025-12-18 |
| `ley-2005-001/` | Ley 1/2005, de 23 de marzo, de creación del Colegio Profesional de Logopedas de Castilla y León. | 1 | as first published: 1 April 2005 | 2025-12-18 |
| `ley-2005-002/` | Ley 2/2005, de 23 de marzo, de creación del Colegio Profesional de Educadores y Educadoras Sociales de Castilla y León. | 1 | as first published: 1 April 2005 | 2025-12-18 |
| `ley-2005-007/` | Ley 7/2005, de 24 de mayo, de la Función Pública de Castilla y León. | 22 | as first published, then each change: 30 June 2005 to 5 December 2025 | 2025-12-18 |
| `ley-2005-008/` | Ley 8/2005, de 10 de junio, de la Viña y del Vino de Castilla y León. | 5 | as first published, then each change: 6 July 2005 to 7 July 2017 | 2025-12-18 |
| `decreto-legislativo-2005-001/` | Decreto Legislativo 1/2005, de 21 de julio, por el que se aprueba el Texto Refundido de la Ley de Cajas de Ahorro de Castilla y León. | 11 | oldest version available, then each change: 28 July 2005 to 18 July 2012 | 2023-12-26 |
| `ley-2005-010/` | Ley 10/2005, de 11 de octubre, de creación del Consejo de Colegios Profesionales de Administradores de Fincas de Castilla y León. | 1 | as first published: 19 October 2005 | 2025-12-18 |
| `ley-2005-012/` | Ley 12/2005, de 27 de diciembre, reguladora del Estatuto de los ex Presidentes de la Junta de Castilla y León. | 1 | as first published: 29 December 2005 | 2025-12-18 |
| `ley-2005-013/` | Ley 13/2005, de 27 de diciembre, de medidas financieras. | 19 | as first published, then each change: 1 January 2006 to 15 May 2024 | 2025-12-18 |
| `ley-2006-001/` | Ley 1/2006, de 6 de abril, de mediación familiar de Castilla y León. | 2 | oldest version available, then each change: 18 October 2006 to 27 December 2009 | 2025-12-18 |
| `ley-2006-002/` | Ley 2/2006, de 3 de mayo, de la Hacienda y del Sector Público de la Comunidad de Castilla y León. | 20 | as first published, then each change: 29 May 2006 to 15 May 2024 | 2025-12-18 |
| `ley-2006-005/` | Ley 5/2006, de 16 de junio, de Cámaras de la Propiedad Urbana de Castilla y León y su Consejo General. | 1 | as first published: 23 June 2006 | 2025-12-18 |
| `ley-2006-006/` | Ley 6/2006, de 5 de julio, de declaración de la Reserva Natural de Lagunas de Villafáfila (Zamora). | 1 | as first published: 15 July 2006 | 2025-12-18 |
| `ley-2006-007/` | Ley 7/2006, de 2 de octubre, de espectáculos públicos y actividades recreativas de la Comunidad de Castilla y León. | 9 | as first published, then each change: 6 January 2007 to 15 May 2024 | 2025-12-18 |
| `ley-2006-008/` | Ley 8/2006, de 10 de octubre, del voluntariado en Castilla y León. | 2 | as first published, then each change: 19 November 2006 to 19 October 2021 | 2025-12-18 |
| `ley-2006-009/` | Ley 9/2006, de 10 de octubre, de cooperación al desarrollo. | 2 | as first published, then each change: 19 November 2006 to 20 September 2014 | 2025-12-18 |
| `ley-2006-010/` | Ley 10/2006, de 14 de octubre, de declaración del Parque Natural de Montes Obarenes-San Zadornil (Burgos). | 1 | as first published: 21 October 2006 | 2025-12-18 |
| `ley-2006-011/` | Ley 11/2006, de 26 de octubre, del patrimonio de la Comunidad de Castilla y León. | 10 | as first published, then each change: 19 November 2006 to 15 May 2024 | 2025-12-18 |
| `ley-2006-012/` | Ley 12/2006, de 26 de octubre, de creación de la empresa pública «Sociedad Pública de Medio Ambiente de Castilla y León». | 8 | as first published, then each change: 3 November 2006 to 15 May 2024 | 2025-12-18 |
| `ley-2007-001/` | Ley 1/2007, de 7 de marzo, de Medidas de Apoyo a las Familias de la Comunidad de Castilla y León. | 4 | oldest version available, then each change: 14 June 2007 to 20 September 2014 | 2025-12-19 |
| `ley-2007-002/` | Ley 2/2007, de 7 de marzo, del Estatuto Jurídico del Personal Estatutario del Servicio de Salud de Castilla y León. | 16 | as first published, then each change: 14 April 2007 to 15 May 2024 | 2025-12-19 |
| `ley-2007-004/` | Ley 4/2007, de 28 de marzo, de Protección Ciudadana de Castilla y León. | 6 | as first published, then each change: 1 May 2007 to 15 May 2024 | 2025-12-19 |
| `ley-2008-003/` | Ley 3/2008, de 17 de junio, de aprobación de las directrices esenciales de ordenación del territorio de Castilla y León. | 3 | as first published, then each change: 25 June 2008 to 4 December 2014 | 2025-12-19 |
| `ley-2008-005/` | Ley 5/2008, de 25 de septiembre, de subvenciones de la Comunidad de Castilla y León. | 11 | as first published, then each change: 4 October 2008 to 15 May 2024 | 2025-12-19 |
| `ley-2008-008/` | Ley 8/2008, de 16 de octubre, para la creación del Consejo del Diálogo Social y regulación de la participación institucional. | 1 | as first published: 24 October 2008 | 2025-12-19 |
| `ley-2008-010/` | Ley 10/2008, de 9 de diciembre, de carreteras de Castilla y León. | 6 | as first published, then each change: 15 January 2009 to 5 December 2025 | 2025-12-19 |
| `ley-2008-011/` | Ley 11/2008, de 9 de diciembre, de declaración de la Reserva Natural "Acebal de Garagüeta" (Soria). | 1 | as first published: 27 December 2008 | 2025-12-19 |
| `ley-2008-012/` | Ley 12/2008, de 9 de diciembre, de declaración del Parque Natural de "Lagunas Glaciares de Neila" (Burgos). | 1 | as first published: 27 December 2008 | 2025-12-19 |
| `ley-2008-014/` | Ley 14/2008, de 18 de diciembre, por la que se crea y regula una red de apoyo a la mujer embarazada. | 1 | as first published: 26 January 2009 | 2025-12-19 |
| `ley-2008-015/` | Ley 15/2008, de 18 de diciembre, de declaración del Parque Natural Hoces del Alto Ebro y Rudrón (Burgos). | 1 | as first published: 27 December 2008 | 2025-12-19 |
| `ley-2008-016/` | Ley 16/2008, de 18 de diciembre, por la que se amplía el Parque Natural de las Batuecas-Sierra de Francia (Salamanca). | 1 | as first published: 27 December 2008 | 2025-12-19 |
| `ley-2009-003/` | Ley 3/2009, de 6 de abril, de montes de Castilla y León. | 15 | as first published, then each change: 16 May 2009 to 5 December 2025 | 2025-12-19 |
| `ley-2009-004/` | Ley 4/2009, de 28 de mayo, de publicidad institucional de Castilla y León. | 4 | as first published, then each change: 30 May 2009 to 12 July 2025 | 2025-12-19 |
| `ley-2009-005/` | Ley 5/2009, de 4 de junio, del ruido de Castilla y León. | 9 | as first published, then each change: 9 August 2009 to 17 March 2021 | 2025-12-19 |
| `ley-2009-008/` | Ley 8/2009, de 16 de junio, de transferencia de competencias entre la Comunidad Autónoma y las Entidades Locales de Castilla y León. | 3 | as first published, then each change: 12 July 2009 to 21 October 2013 | 2025-12-19 |
| `ley-2010-001/` | Ley 1/2010, de 2 de marzo, de declaración del parque natural de "Laguna Negra y Circos Glaciares de Urbión" (Soria). | 1 | as first published: 11 March 2010 | 2025-12-19 |
| `ley-2010-002/` | Ley 2/2010, de 11 de marzo, de Derechos de los Ciudadanos en sus relaciones con la Administración de la Comunidad de Castilla y León y de Gestión Pública. | 3 | as first published, then each change: 22 April 2010 to 7 July 2017 | 2025-12-19 |
| `ley-2010-008/` | Ley 8/2010, de 30 de agosto, de ordenación del sistema de salud de Castilla y León. | 12 | as first published, then each change: 8 September 2010 to 20 January 2026 | 2026-01-20 |
| `ley-2010-009/` | Ley 9/2010, de 30 de agosto, del derecho a la vivienda de la Comunidad de Castilla y León. | 10 | as first published, then each change: 8 September 2010 to 15 May 2024 | 2025-12-19 |
| `ley-2010-010/` | Ley 10/2010, de 27 de septiembre, de salud pública y seguridad alimentaria de Castilla y León. | 5 | as first published, then each change: 9 October 2010 to 24 October 2020 | 2025-12-19 |
| `ley-2010-011/` | Ley 11/2010, de 11 de octubre, de creación del Colegio Profesional de Terapeutas Ocupacionales de Castilla y León. | 2 | as first published, then each change: 22 October 2010 to 1 March 2012 | 2025-12-19 |
| `ley-2010-013/` | Ley 13/2010, de 9 de diciembre, contra la violencia de género en Castilla y León. | 2 | as first published, then each change: 21 December 2010 to 1 January 2018 | 2025-12-19 |
| `ley-2010-014/` | Ley 14/2010, de 9 de diciembre, de turismo de Castilla y León. | 5 | as first published, then each change: 20 March 2011 to 17 March 2021 | 2025-12-19 |
| `ley-2010-015/` | Ley 15/2010, de 10 de diciembre, de prevención de la contaminación lumínica y del fomento del ahorro y eficiencia energéticos derivados de instalaciones de iluminación. | 3 | as first published, then each change: 9 January 2011 to 7 July 2017 | 2025-12-19 |
| `ley-2010-016/` | Ley 16/2010, de 20 de diciembre, de servicios sociales de Castilla y León. | 12 | as first published, then each change: 21 March 2011 to 20 February 2024 | 2025-12-19 |
| `ley-2010-018/` | Ley 18/2010, de 20 de diciembre, de declaración del Parque Natural "Sierra Norte de Guadarrama" (Segovia y Ávila). | 1 | as first published: 22 December 2010 | 2025-12-19 |
| `ley-2011-001/` | Ley 1/2011, de 1 de marzo, de evaluación del impacto de género en Castilla y León. | 1 | as first published: 11 July 2011 | 2025-12-19 |
| `ley-2011-003/` | Ley 3/2011, de 22 de marzo, por la que se reconoce como universidad privada a la "Universidad Privada Internacional de Burgos", con sede en Burgos. | 2 | as first published, then each change: 20 April 2011 to 11 May 2012 | 2025-12-19 |
| `ley-2011-004/` | Ley 4/2011, de 29 de marzo, de aprobación de las Directrices de Ordenación de Ámbito Subregional de la Montaña Cantábrica Central en Castilla y León. | 1 | as first published: 15 April 2011 | 2025-12-19 |
| `ley-2012-007/` | Ley 7/2012, de 24 de octubre, de Estabilidad y Disciplina Presupuestaria. | 3 | as first published, then each change: 3 November 2012 to 1 January 2015 | 2025-12-19 |
| `decreto-ley-2012-002/` | Decreto-ley 2/2012, de 25 de octubre, por el que se adoptan medidas urgentes en materia Sanitaria. | 1 | oldest version available: 30 October 2012 | 2023-12-26 |
| `ley-2012-008/` | Ley 8/2012, de 8 de noviembre, de creación del Colegio Profesional de Periodistas de Castilla y León. | 1 | as first published: 15 November 2012 | 2025-12-19 |
| `ley-2013-002/` | Ley 2/2013, de 15 de mayo, de Igualdad de Oportunidades para las Personas con Discapacidad. | 3 | as first published, then each change: 13 June 2013 to 20 February 2024 | 2025-12-19 |
| `ley-2013-003/` | Ley 3/2013, de 28 de mayo, de integración de los inmigrantes en la sociedad de Castilla y León. | 2 | as first published, then each change: 6 June 2013 to 20 September 2014 | 2025-12-19 |
| `ley-2013-005/` | Ley 5/2013, de 19 de junio, de Estímulo a la Creación de Empresas en Castilla y León. | 3 | as first published, then each change: 4 July 2013 to 2 September 2014 | 2025-12-19 |
| `decreto-legislativo-2013-001/` | Decreto Legislativo 1/2013, de 12 de septiembre, por el que se aprueba el texto refundido de las disposiciones legales de la Comunidad de Castilla y León en materia de tributos propios y cedidos. | 17 | oldest version available, then each change: 19 September 2013 to 15 May 2024 | 2024-07-17 |
| `ley-2013-007/` | Ley 7/2013, de 27 de septiembre, de Ordenación, Servicios y Gobierno del Territorio de la Comunidad de Castilla y León. | 5 | as first published, then each change: 21 October 2013 to 17 March 2021 | 2025-12-19 |
| `ley-2013-008/` | Ley 8/2013, de 29 de octubre, de la Ciudadanía Castellana y Leonesa en el Exterior. | 1 | as first published: 25 November 2013 | 2026-03-20 |
| `ley-2013-009/` | Ley 9/2013, de 3 de diciembre, de Pesca de Castilla y León. | 5 | as first published, then each change: 2 January 2014 to 15 May 2024 | 2025-12-19 |
| `ley-2013-010/` | Ley 10/2013, de 16 de diciembre, de medidas urgentes en materia de Vivienda. | 2 | as first published, then each change: 21 December 2013 to 19 October 2014 | 2025-12-19 |
| `ley-2014-001/` | Ley 1/2014, de 19 de marzo, Agraria de Castilla y León. | 6 | as first published, then each change: 21 March 2014 to 15 May 2024 | 2025-12-19 |
| `ley-2014-002/` | Ley 2/2014, de 28 de marzo, de Centros Museísticos de Castilla y León. | 1 | as first published: 3 June 2014 | 2025-12-19 |
| `ley-2014-003/` | Ley 3/2014, de 16 de abril, de autoridad del profesorado. | 1 | as first published: 3 May 2014 | 2025-12-19 |
| `ley-2014-004/` | Ley 4/2014, de 9 de mayo, de creación del Colegio Profesional de Dietistas-Nutricionistas de Castilla y León. | 1 | as first published: 23 May 2014 | 2025-12-19 |
| `decreto-legislativo-2014-002/` | Decreto Legislativo 2/2014, de 28 de agosto, por el que se aprueba el texto refundido de la Ley de Comercio de Castilla y León. | 2 | oldest version available, then each change: 2 September 2014 to 7 July 2017 | 2023-12-26 |
| `ley-2014-006/` | Ley 6/2014, de 12 de septiembre, de Industria de Castilla y León. | 1 | as first published: 19 October 2014 | 2025-12-19 |
| `ley-2014-007/` | Ley 7/2014, de 12 de septiembre, de Medidas sobre Rehabilitación, Regeneración y Renovación Urbana, y sobre Sostenibilidad, Coordinación y Simplificación en Materia de Urbanismo. | 3 | as first published, then each change: 19 October 2014 to 15 May 2024 | 2025-12-19 |
| `ley-2014-009/` | Ley 9/2014, de 27 de noviembre, por la que se declaran las áreas funcionales estables de Castilla y León y se modifica la Ley 7/2013, de 27 de septiembre, de Ordenación, Servicios y Gobierno del Territorio de la Comunidad de Castilla y León. | 2 | as first published, then each change: 4 December 2014 to 11 July 2018 | 2025-12-19 |
| `ley-2015-002/` | Ley 2/2015, de 4 de marzo, por la que se aprueba el Estatuto del Consumidor de Castilla y León. | 4 | as first published, then each change: 1 April 2015 to 28 April 2018 | 2025-12-19 |
| `ley-2015-003/` | Ley 3/2015, de 4 de marzo, de Transparencia y Participación Ciudadana de Castilla y León. | 4 | as first published, then each change: 13 March 2015 to 17 March 2021 | 2025-12-19 |
| `ley-2015-004/` | Ley 4/2015, de 24 de marzo, del Patrimonio Natural de Castilla y León. | 6 | as first published, then each change: 19 April 2015 to 5 December 2025 | 2025-12-19 |
| `ley-2015-005/` | Ley 5/2015, de 24 de marzo, de declaración del Parque Natural de "Babia y Luna" (León). | 1 | as first published: 31 March 2015 | 2025-12-19 |
| `ley-2015-006/` | Ley 6/2015, de 24 de marzo, de creación del Consejo de Colegios Profesionales de Odontólogos y Estomatólogos de Castilla y León. | 1 | as first published: 31 March 2015 | 2025-12-19 |
| `decreto-legislativo-2015-001/` | Decreto legislativo 1/2015, de 12 de noviembre, por el que se aprueba el texto refundido de la Ley de Prevención Ambiental de Castilla y León. | 6 | oldest version available, then each change: 14 November 2015 to 15 May 2024 | 2024-10-28 |
| `decreto-ley-2016-002/` | Decreto-ley 2/2016, de 19 de mayo, por el que se prohíbe la muerte de las reses de lidia en presencia del público en los espectáculos taurinos populares y tradicionales en Castilla y León. | 1 | oldest version available: 20 May 2016 | 2023-12-26 |
| `ley-2016-003/` | Ley 3/2016, de 30 de noviembre, del Estatuto de los Altos Cargos de la Administración de la Comunidad de Castilla y León. | 1 | as first published: 14 January 2017 | 2025-12-19 |
| `ley-2016-004/` | Ley 4/2016, de 23 de diciembre, por la que se adoptan medidas para reforzar la cobertura de las necesidades de atención social en el ámbito de la Red de Protección a las Familias de Castilla y León afectadas por la crisis. | 3 | as first published, then each change: 30 December 2016 to 16 January 2019 | 2025-12-19 |
| `ley-2017-001/` | Ley 1/2017, de 28 de marzo, por la que se amplían los límites del Parque Natural Lago de Sanabria y alrededores (Zamora), se modifica su denominación por la de Parque Natural Lago de Sanabria y Sierras Segundera y de Porto (Zamora), y se establece su régimen de protección, uso y gestión. | 1 | as first published: 6 April 2017 | 2025-12-19 |
| `ley-2017-004/` | Ley 4/2017, de 26 de septiembre, de reconocimiento y atención a las víctimas del terrorismo en Castilla y León. | 1 | as first published: 3 October 2017 | 2025-12-19 |
| `ley-2017-005/` | Ley 5/2017, de 17 de octubre, de creación del Ilustre Colegio Profesional de Economistas de Valladolid por fusión del Colegio Oficial de Economistas de Valladolid con el Colegio Oficial de Titulares Mercantiles de Valladolid y de creación del Ilustre Colegio Profesional de Economistas de Burgos por fusión del Colegio Oficial de Economistas de Burgos con el Colegio Oficial de Titulares Mercantiles de Burgos. | 1 | as first published: 26 October 2017 | 2025-12-19 |
| `ley-2017-006/` | Ley 6/2017, de 20 de octubre, de medidas de reducción de cargas administrativas para la dinamización empresarial. | 1 | as first published: 26 October 2017 | 2025-12-19 |
| `ley-2018-003/` | Ley 3/2018, de 2 de julio, por el que se modifica la Ley 9/2003, de 8 de abril, de Coordinación de Policías Locales de Castilla y León. | 1 | as first published: 30 July 2018 | 2025-12-20 |
| `ley-2018-004/` | Ley 4/2018, de 2 de julio, de ordenación y funcionamiento de la red de protección e inclusión a personas y familias en situación de mayor vulnerabilidad social o económica en Castilla y León. | 4 | as first published, then each change: 11 July 2018 to 22 October 2022 | 2025-12-20 |
| `decreto-ley-2018-003/` | Decreto-ley 3/2018, de 30 de agosto, por el que se habilita el incremento de las retribuciones y se eliminan las limitaciones para el abono del 100% en las situaciones de incapacidad temporal del personal al servicio del sector público. | 1 | oldest version available: 4 September 2018 | 2026-05-25 |
| `ley-2018-007/` | Ley 7/2018, de 14 de diciembre, por la que se regula la Conferencia de Titulares de Alcaldías y Presidencias de Diputación, el estatuto de los miembros de las entidades locales y la información en los Plenos. | 1 | as first published: 16 January 2019 | 2025-12-20 |
| `ley-2018-008/` | Ley 8/2018, de 14 de diciembre, por la que se regulan las Cámaras Oficiales de Comercio, Industria y Servicios de Castilla y León y el Consejo de Cámaras de Castilla y León. | 1 | as first published: 16 January 2019 | 2025-12-20 |
| `ley-2018-009/` | Ley 9/2018, de 20 de diciembre, de transporte público de viajeros por carretera de Castilla y León. | 2 | as first published, then each change: 3 July 2019 to 20 June 2020 | 2025-12-20 |
| `decreto-legislativo-2019-001/` | Decreto Legislativo 1/2019, de 10 de enero, por el que se aprueba el texto refundido de las normas legales vigentes en materia de condiciones de acceso y disfrute de la prestación de renta garantizada de ciudadanía de Castilla y León. | 2 | oldest version available, then each change: 16 January 2019 to 4 December 2020 | 2023-12-26 |
| `ley-2019-003/` | Ley 3/2019, de 25 de febrero, de la Actividad Físico-Deportiva de Castilla y León. | 2 | as first published, then each change: 5 June 2019 to 17 March 2021 | 2025-12-20 |
| `decreto-ley-2019-001/` | Decreto-ley 1/2019, de 28 de febrero, sobre medidas urgentes en materia de sanidad. | 3 | oldest version available, then each change: 5 March 2019 to 20 January 2026 | 2026-04-17 |
| `ley-2019-004/` | Ley 4/2019, de 19 de marzo, por el que se modifica la Ley 2/2007, de 7 de marzo, del Estatuto Jurídico del Personal Estatutario del Servicio de Salud de Castilla y León, para la creación de la categoría de Médico de Cuidados Paliativos. | 1 | as first published: 27 March 2019 | 2025-12-20 |
| `ley-2019-007/` | Ley 7/2019, de 19 de marzo, de implantación y desarrollo de la carrera profesional de los empleados públicos de la Administración de la Comunidad de Castilla y León. | 3 | as first published, then each change: 26 April 2019 to 15 May 2024 | 2025-12-20 |
| `ley-2019-010/` | Ley 10/2019, de 3 de abril, por la que se promueve la adopción en el ámbito público y privado de medidas dirigidas a la conciliación de la vida personal, familiar y laboral y a la eliminación de la brecha salarial de género en Castilla y León. | 1 | as first published: 9 April 2019 | 2025-12-20 |
| `ley-2019-011/` | Ley 11/2019, de 3 de abril, de acceso al entorno de las personas usuarias de perro de asistencia en la Comunidad de Castilla y León | 1 | as first published: 8 October 2019 | 2025-12-20 |
| `decreto-ley-2020-007/` | Decreto-ley 7/2020, de 23 de julio, por el que se establece el régimen sancionador específico por el incumplimiento de las medidas de prevención y contención sanitarias para afrontar la situación de crisis sanitaria ocasionada por la COVID-19 en la Comunidad de Castilla y León. | 3 | oldest version available, then each change: 25 July 2020 to 27 March 2021 | 2026-02-03 |
| `decreto-ley-2020-008/` | Decreto-ley 8/2020, de 3 de septiembre, por el que se modifica la Ley 7/2006, de 2 de octubre, de Espectáculos Públicos y Actividades Recreativas de la Comunidad de Castilla y León. | 1 | oldest version available: 4 September 2020 | 2023-12-26 |
| `decreto-ley-2020-009/` | Decreto-ley 9/2020, de 10 de septiembre, por el que se adoptan medidas extraordinarias de apoyo a las personas y familias para la atención domiciliaria de menores, personas dependientes o con discapacidad que deban guardar confinamiento domiciliario a causa de la pandemia COVID 19. | 1 | oldest version available: 11 September 2020 | 2024-06-14 |
| `decreto-ley-2020-010/` | Decreto-ley 10/2020, de 22 de octubre, de medidas urgentes para reforzar el control y sanción de las medidas de prevención y contención sanitarias para afrontar la situación de crisis sanitaria ocasionada por la COVID-19. | 1 | oldest version available: 24 October 2020 | 2024-06-13 |
| `ley-2020-004/` | Ley 4/2020, de 14 de diciembre, de declaración del Parque Natural de "Sabinares del Arlanza-La Yecla" (Burgos). | 1 | as first published: 10 January 2021 | 2025-12-20 |
| `decreto-ley-2021-001/` | Decreto-ley 1/2021, de 18 de marzo, de medidas urgentes y extraordinarias para el sostenimiento y reactivación de los sectores turístico y deportivo de Castilla y León frente al impacto económico y social de la COVID-19. | 1 | oldest version available: 20 March 2021 | 2024-05-09 |
| `ley-2021-004/` | Ley 4/2021, de 1 de julio, de Caza y de Gestión Sostenible de los Recursos Cinegéticos de Castilla y León. | 4 | as first published, then each change: 8 August 2021 to 15 May 2024 | 2026-06-26 |
| `ley-2021-005/` | Ley 5/2021, de 14 de septiembre, del Tercer Sector Social en Castilla y León y de modificación de la Ley 8/2006, de 10 de octubre, del Voluntariado en Castilla y León. | 1 | as first published: 19 October 2021 | 2025-12-20 |
| `decreto-ley-2022-002/` | Decreto-ley 2/2022, de 23 de junio, por el que se adoptan medidas urgentes para la agilización de la gestión de los fondos europeos y el impulso de la actividad económica. | 2 | oldest version available, then each change: 25 June 2022 to 29 October 2022 | 2024-04-23 |
| `decreto-ley-2022-004/` | Decreto-ley 4/2022, de 27 de octubre, de modificación del Decreto-Legislativo 1/2015, de 12 de noviembre, por el que se aprueba el texto refundido de la Ley de Prevención Ambiental de Castilla y León, del Decreto-Ley 2/2022, de 23 de junio, por el que se adoptan medidas urgentes para la agilización de la gestión de los fondos europeos y el impulso de la actividad económica y por el que se actualizan las retribuciones para 2022 en el ámbito del sector público de la Comunidad Autónoma de Castilla y León. | 1 | oldest version available: 29 October 2022 | 2024-04-19 |
| `decreto-ley-2023-003/` | Decreto-ley 3/2023, de 11 de mayo, por el que se regula el Sistema Interno de Información de la Administración de la Comunidad de Castilla y León. | 1 | oldest version available: 16 May 2023 | 2024-04-19 |
| `ley-2024-001/` | Ley 1/2024, de 8 de febrero, de apoyo al proyecto de vida de las personas con discapacidad en Castilla y León. | 1 | as first published: 20 February 2024 | 2025-12-20 |
| `ley-2024-003/` | Ley 3/2024, de 12 de abril, reguladora del modelo de atención en los centros de carácter residencial y centros de día de servicios sociales para cuidados de larga duración en Castilla y León. | 1 | as first published: 14 May 2024 | 2025-12-20 |
| `ley-2024-007/` | Ley 7/2024, de 20 de junio, de Patrimonio Cultural de Castilla y León. | 1 | as first published: 27 September 2024 | 2025-12-20 |
| `ley-1996-004/` | Ley 4/1996, de 12 de julio, de Caza de Castilla y León. | 14 | oldest version available, then each change: 22 October 1996 to 8 August 2021; **repealed** 8 August 2021 by Ley 4/2021, de 1 de julio (BOE-A-2021-12058) | 2025-12-18 |
| `ley-2002-012/` | Ley 12/2002, de 11 de julio, de Patrimonio Cultural de Castilla y León. | 5 | as first published, then each change: 8 August 2002 to 27 September 2024; **repealed** 27 September 2024 by Ley 7/2024, de 20 de junio (BOE-A-2024-15102) | 2026-10-27 |
| `ley-2002-016/` | Ley 16/2002, de 19 de diciembre, de Comercio de Castilla y León. | 7 | as first published, then each change: 13 January 2003 to 2 September 2014; **repealed** 2 September 2014 by Decreto Legislativo 2/2014, de 28 de agosto (BOCL-h-2014-90371) | 2025-12-18 |
| `ley-2003-011/` | Ley 11/2003, de 8 de abril, de Prevención Ambiental de Castilla y León. | 11 | as first published, then each change: 14 June 2003 to 14 November 2015; **repealed** 14 November 2015 by Decreto legislativo 1/2015, de 12 de noviembre (BOCL-h-2015-90590) | 2025-12-18 |
| `decreto-legislativo-2014-001/` | Decreto Legislativo 1/2014, de 27 de febrero, por el que se aprueba el texto refundido de las normas legales vigentes en materia de condiciones de acceso y disfrute de la prestación esencial de renta garantizada de ciudadanía de Castilla y León. | 5 | oldest version available, then each change: 4 March 2014 to 16 January 2019; **repealed** 16 January 2019 by Decreto Legislativo 1/2019, de 10 de enero (BOCL-h-2019-90258) | 2023-12-26 |
| `ley-2016-002/` | Ley 2/2016, de 11 de noviembre, por la que se regulan las actuaciones para dar curso a las informaciones que reciba la Administración Autonómica sobre hechos relacionados con delitos contra la Administración Pública y se establecen las garantías de los informantes. | 2 | as first published, then each change: 22 November 2016 to 16 May 2023; **repealed** 16 May 2023 by Decreto-ley 3/2023, de 11 de mayo (BOCL-h-2023-90202) | 2025-12-19 |
| `decreto-ley-2020-005/` | Decreto-ley 5/2020, de 18 de junio, por el que se regulan las medidas extraordinarias que deben adoptarse en la atención social en los centros residenciales de personas mayores y personas con discapacidad en Castilla y León para garantizar la protección de usuarios y profesionales ante situaciones excepcionales de salud pública declaradas oficialmente. | 2 | oldest version available, then each change: 19 June 2020 to 14 May 2024; **repealed** 14 May 2024 by Ley 3/2024, de 12 de abril (BOE-A-2024-8834) | 2024-06-17 |
| `acuerdo-2020-111/` | Acuerdo 111/2020, de 30 de diciembre, de la Junta de Castilla y León, por el que se aprueban los estatutos de la Universidad de Valladolid. | 2 | as first published, then each change: 1 January 2021 to 12 March 2026; **repealed** 12 March 2026 by Acuerdo 23/2026 de 5 de marzo de 2026 (BOE-A-2026-6406) | 2026-03-19 |

## Source

The consolidated legislation of the Agencia Estatal Boletín Oficial del Estado (BOE), through its open-data API, <https://www.boe.es/datosabiertos/api/legislacion-consolidada>. For each consolidated norm it gives every block of the text (article, disposition, annex, heading) with every version of that block, the day each version took effect (fecha_vigencia) and the norm that made it (id_norma). Each version here is the whole text as it stood on one of those days. The last column above is the BOE's own last-update date for the consolidated text.

## Dates

- Each commit is dated at **noon, Europe/Madrid, on the day the change took effect**: the fecha_vigencia the BOE gives the new block versions.
- A day on which the BOE records a new block version that changes no words is not a version here.
- Block versions with no in-force date (the BOE's 99999999, a date not yet fixed) are left out.
- An act's first commit is its first publication when the BOE's earliest text is the act as enacted; otherwise it is the oldest version the BOE holds.
- Versions that take effect after the retrieval day are on the `futuro` branch, never merged into `main`.

## Files

`<act>/art-005.md` is Artículo 5, `art-005-bis.md` Artículo 5 bis; `da-01.md` the Disposición adicional primera, `dt-` transitional, `dd-` repealing and `df-` final dispositions (`-unica` for "única"); `preambulo.md` the preamble, `firma.md` the signature, `anexo-*.md` the annexes. The book, title, chapter and section headings sit at the top of the file of the article that follows them. One paragraph per line; a table one line per row, cells separated by ` | `.

## How it is checked

- Every version of every act is read back from git on the day it took effect and on the day before (`tools/check_repo.py`); both must match `corpus.json`.
- The letters and digits of every version equal those of the BOE's own text of that day, rebuilt from the source XML by a separate reader, and every file's text appears in it.
- Health checks: no merge commits, commit dates never go backwards, nothing dated in the future, and every commit's trailers parse.

## What "author" means

The author of a commit is the norm that changed the text (a law, a decree-law, a ruling of the Constitutional Court), named by its title and BOE identifier, with an e-mail address that cannot exist (`<boe id>@boe.es.invalid`). The committer is always Lexifina.

## Limits

This is not an official publication. Only the texts published in the official journals are authentic. The history starts with the oldest text the BOE consolidates for each norm. Only the norms listed above are included; norms the BOE does not consolidate are not.
