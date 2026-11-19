# come funziona la PROMISE

1. si parte con il recupero del file. *fetch()* restituisce una **promise**: prometto che quando lo ho ti do il file!     


        fetch("file.txt");



2. serve tempo, aspetta che provvedo, ok?


        await fetch("file.txt");


3. questo file va restituito in una **response**


        const response = await fetch("file.txt");


4. per ottenere il contenuto del file, mi serve un'altra promise: per accedere al file mi serve tempo!


        let fileContent = await response.text();


