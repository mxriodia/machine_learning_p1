# Procedencia y licencia de los datos — Práctica 1, grupo 4

## Los cuadros

| Campo | Valor |
|---|---|
| Fuente | Art Institute of Chicago, colección en línea (<https://www.artic.edu/collection>) |
| Licencia | **Creative Commons Zero (CC0)**: el museo ofrece estas imágenes, de obras que considera de dominio público, para uso libre y sin restricciones (<https://www.artic.edu/open-access/open-access-images>) |
| Metadatos | También CC0, según la API pública del museo (<https://api.artic.edu/docs/>) |
| Descarga | 23 de octubre de 2026, mediante la API pública (versión de 843 píxeles de ancho) |
| Ficheros | 56 JPEG, lado mayor de 512 píxeles, calidad 90; 3063831 bytes en total |

**El curso no ha creado estas obras ni sus reproducciones.** Lo propio del curso es la selección,
el cambio de tamaño y la organización en dos tablas.

**Selección.** Cada grupo tiene seis autores: uno que pinta sobre papel o en laca, y cinco al óleo.
De cada autor se tomaron hasta diez obras de dominio público con imagen y fecha, por orden creciente
de identificador del museo. Los autores con muchas obras se repartieron en tramos distintos entre
los grupos. El orden de las filas se barajó, de modo que ni `row_id` ni el nombre del fichero
revelan el autor.

| Fichero | Contenido | Cuándo se usa | Bytes | SHA-256 |
|---|---|---|---:|---|
| `cuadros.csv` | `row_id`, `fichero`, `ancho`, `alto` | toda la práctica | 1417 | `373e386010f4499406b14dfaff36f8b21007dbcb916cc2466332016abfdb2bb6` |
| `grupo.json` | número de grupo y `row_id` de los tres cuadros del Ejercicio 1 | toda la práctica | 72 | `2031d77c54117b4e7024bf6594ca832d89f0fe601ac411a0eecb5d74f53cbfff` |
| `metadatos.csv` | `row_id`, `autor`, `epoca`, `anio`, `tecnica`, `titulo`, `tecnica_original`, `aic_id` | **solo en la revelación** | 5784 | `78da96f6c542b624619a99b45f4b12499ffcc3c919bda81ff3a71c75ece7fa4f` |

- `epoca` agrupa el año de inicio que da el museo (`anio`) en cinco tramos: antes de 1800,
  1800-1849, 1850-1874, 1875-1899 y 1900 o después.
- `tecnica` resume la técnica en tres valores: óleo, tinta sobre papel o seda, y laca sobre papel.
- `titulo` y `tecnica_original` son los valores del museo y se dejan sin traducir.

### Lista de obras

El museo pide citar sus imágenes como *Artista. Título, fecha. The Art Institute of Chicago.*
La lista va por autor, no por `row_id`, para que este fichero no sirva de atajo antes de la
revelación. **Contiene los nombres de los autores: si queréis que la revelación sea una sorpresa,
no la leáis antes.**

| Autor | Título | Fecha | Id. del museo | Procedencia (credit line) |
|---|---|---|---:|---|
| Claude Monet | Boats on the Beach at Étretat | 1885 | 59927 | Charles H. and Mary F. S. Worcester Collection |
| Claude Monet | Stacks of Wheat (End of Summer) | 1890–91 | 64818 | Gift of Arthur M. Wood, Sr. in memory of Pauline Palmer Wood |
| Claude Monet | Bordighera | 1884 | 81537 | Potter Palmer Collection |
| Claude Monet | On the Bank of the Seine, Bennecourt | 1868 | 81539 | Potter Palmer Collection |
| Claude Monet | The Departure of the Boats, Étretat | 1885 | 81540 | Potter Palmer Collection |
| Claude Monet | Stacks of Wheat (Sunset, Snow Effect) | 1890–91 | 81545 | Potter Palmer Collection |
| Claude Monet | The Petite Creuse River | 1889 | 81546 | Potter Palmer Collection |
| Claude Monet | Sandvika, Norway | 1895 | 86998 | Gift of Bruce Borland |
| Claude Monet | Water Lily Pond | 1900 | 87088 | Mr. and Mrs. Lewis Larned Coburn Memorial Collection |
| Claude Monet | Water Lily Pond | 1917–19 | 97933 | Gift of Mrs. Harvey Kaplan |
| James McNeill Whistler | Study for "Arrangement in Grey and Black, No. 2: Portrait of Thomas Carlyle" | 1872–73 | 3551 | Gift of Emily Crane Chadbourne |
| James McNeill Whistler | Arrangement in Flesh Color and Brown: Portrait of Arthur Jerome Eddy | 1894 | 8958 | Arthur Jerome Eddy Memorial Collection |
| James McNeill Whistler | Coast Scene, Bathers | 1884–85 | 14309 | Walter S. Brewster Collection |
| James McNeill Whistler | Study of a Girl's Head and Shoulders | 1896–97 | 14317 | Walter S. Brewster Collection |
| James McNeill Whistler | Nocturne: Blue and Gold—Southampton Water | 1872 | 56905 | Stickney Fund |
| James McNeill Whistler | The Artist in His Studio | 1865–66 | 65709 | Friends of American Art Collection |
| James McNeill Whistler | Trouville (Grey and Green, the Silver Sea) | 1865 | 81572 | Gift of Honoré and Potter Palmer |
| James McNeill Whistler | Grey and Silver: Old Battersea Reach | 1863 | 81574 | Gift of Honoré and Potter Palmer |
| James McNeill Whistler | Violet and Silver—The Deep Sea | 1893 | 84088 | Gift of Clara Margaret Lynch in memory of John A. Lynch |
| James McNeill Whistler | Portrait of Dr. William McNeill Whistler | 1871–73 | 111478 | Gift of Mary T. Wentworth in memory of her husband, John |
| Jean François Millet | The Keeper of the Flock | 1871–74 | 4776 | Mr. and Mrs. W. W. Kimball Collection |
| Jean François Millet | The Little Shepherdess | 1868–72 | 81515 | Potter Palmer Collection |
| Jean François Millet | In the Auvergne | c. 1866–69 | 81516 | Potter Palmer Collection |
| Jean François Millet | Young Woman | 1844–45 | 81519 | Potter Palmer Collection |
| Jean François Millet | The Woodchopper | c. 1858–66 | 81521 | Potter Palmer Collection |
| Jean François Millet | The Sheepshearers | c. 1857–61 | 81522 | Potter Palmer Collection |
| Jean François Millet | Woman Feeding Chickens | 1846-48 | 111646 | Henry Field Memorial Collection |
| Jean François Millet | Peasants Bringing Home a Calf Born in the Fields | 1864 | 111648 | Henry Field Memorial Collection |
| Marsden Hartley | The Dark Mountain | 1909 | 65908 | Alfred Stieglitz Collection |
| Marsden Hartley | Landscape no. 26 | 1909–10 | 65912 | Alfred Stieglitz Collection |
| Marsden Hartley | Movement | 1913 | 65916 | Alfred Stieglitz Collection |
| Marsden Hartley | Provincetown | 1916 | 65920 | Alfred Stieglitz Collection |
| Marsden Hartley | The Last of New England—The Beginning of New Mexico | 1918–19 | 65925 | Alfred Stieglitz Collection |
| Marsden Hartley | Still Life No. 15 | c. 1917 | 65930 | Alfred Stieglitz Collection |
| Marsden Hartley | Landscape No. 3, Cash Entry Mines, New Mexico | 1920 | 65937 | Alfred Stieglitz Collection |
| Marsden Hartley | Still Life No. 3 | 1923 | 65940 | Alfred Stieglitz Collection |
| Marsden Hartley | Movement No. 10 | 1917 | 90207 | Alfred Stieglitz Collection |
| Paul Cezanne | Auvers, Panoramic View | 1873–75 | 14556 | Mr. and Mrs. Lewis Larned Coburn Memorial Collection |
| Paul Cezanne | The Vase of Tulips | c. 1890 | 14561 | Mr. and Mrs. Lewis Larned Coburn Memorial Collection |
| Paul Cezanne | The Bay of Marseille, Seen from L'Estaque | c. 1885 | 16487 | Mr. and Mrs. Martin A. Ryerson Collection |
| Paul Cezanne | The Bathers | 1899-1904 | 45240 | Amy McCormick Memorial Collection |
| Paul Cezanne | Madame Cezanne in a Yellow Chair | 1888–90 | 62371 | Wilson L. Mead Fund |
| Paul Cezanne | The Plate of Apples | c. 1877 | 65811 | Gift of Kate L. Brewster |
| Paul Cezanne | Bathers | 1890–94 | 109418 | Gift of Mrs. T. Clifford Rodman |
| Paul Cezanne | The Basket of Apples | c. 1893 | 111436 | Helen Birch Bartlett Memorial Collection |
| Paul Cezanne | Standing Bather, Seen from the Back | 1879-82 | 191564 | Bequest of Brooks McCormick |
| Xugu | Calligraphy Accompanying Xugu's Painting | Qing dynasty (1644–1911), 1897 | 217674 | Gift of Florence Ayscough and Harley Farnsworth MacNair |
| Xugu | Album of Landscapes and Calligraphy for Liu Songfu | Qing dynasty (1644–1911), 1895/96 | 217675 | Gift of Florence Ayscough and Harley Farnsworth MacNair |
| Xugu | Calligraphy Accompanying Xugu's Painting | Qing dynasty (1644–1911), 1897 | 217676 | Gift of Florence Ayscough and Harley Farnsworth MacNair |
| Xugu | Album of Landscapes and Calligraphy for Liu Songfu | Qing dynasty (1644–1911), 1895/96 | 217677 | Gift of Florence Ayscough and Harley Farnsworth MacNair |
| Xugu | Calligraphy Accompanying Xugu's Painting | Qing dynasty (1644–1911), 1897 | 217678 | Gift of Florence Ayscough and Harley Farnsworth MacNair |
| Xugu | Album of Landscapes and Calligraphy for Liu Songfu | Qing dynasty (1644–1911), 1895/96 | 217679 | Gift of Florence Ayscough and Harley Farnsworth MacNair |
| Xugu | Calligraphy Accompanying Xugu's Painting | Qing dynasty (1644–1911), 1897 | 217680 | Gift of Florence Ayscough and Harley Farnsworth MacNair |
| Xugu | Album of Landscapes and Calligraphy for Liu Songfu | Qing dynasty (1644–1911), 1895/96 | 217681 | Gift of Florence Ayscough and Harley Farnsworth MacNair |
| Xugu | Calligraphy Accompanying Xugu's Painting | Qing dynasty (1644–1911), 1897 | 217682 | Gift of Florence Ayscough and Harley Farnsworth MacNair |
| Xugu | Album of Landscapes and Calligraphy for Liu Songfu | Qing dynasty (1644–1911), 1895/96 | 217683 | Gift of Florence Ayscough and Harley Farnsworth MacNair |
