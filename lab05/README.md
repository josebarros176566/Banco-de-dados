

MATCH(m:Marcador)-[:Pertence]->(c:Categoria{id:'Serviços'}) RETURN m

MATCH(m:Marcador)-[:Pertence]->(c:Categoria)-[:Superior]->(d:Categoria{id:'Serviços'}) MATCH(b:Marcador)-[:Pertence]->(e:Categoria{id:'Serviços'}) RETURN m, b
