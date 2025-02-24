# EasyATP

## Urratsak:

1. Saio berri bat ireki zure [https://github.com/](https://github.com/) kontuan, edo sortu kontu berri bat. 

2. Erabili zure edozein biltegi (repository), edo sortu biltegi berri bat.

    ![2a. Create a new repository](/images/CreateNewCodespace.png "2a. Create a new repository")
    
    ![2b. Set new repository name](/images/CreateNewRepositorySetName.png "2b. Set new repository name")
    
    ![2c. Save new repository](/images/CreateNewRepositorySaveButton.png "2c. Save new repository")

3. Sortu codespace berri bat. Zure biltegia hutsa bada (berria), JavierAlvez/EasyATP biltegia (honako hau) klonatu ahal duzu:

    ![3a. Create a new codespace](/images/CreateNewCodespace.png "3a. Create a new codespace")
    
    ![3b. Select a non-empty repository](/images/CreateNewCodespaceSelectRepository.png "3b. Select a non-empty repository")
    
    ![3c. Save new repository](/images/CreateNewCodespaceCreateButton.png "3c. Save new repository")

4. Terminal lehioan hurrengo komandoa exekutatu:

    ```shell
    docker run --name easyatp -p 3000:3000 -d javieralvez/easyatp:2024
    ```

    ![4. Execute Docker Run Command](/images/DockerRunCommand.png "4. Execute Docker Run Command")

5. Ireki EasyATP fitxa berri batean "Open in Browser" botoia sakatuz:

    ![5. Open in browser](/images/DockerRunCommand.png "5. Open in browser")

6. EasyATP tresnarekin lan egin:

    ![6. Ready to work](/images/DockerRunCommand.png "6. Ready to work")

7. Bukatzeko, lan egin eta gero, gelditu codespace. Azken hau oso garrantzitsua da, hilabetero 2000 minutu bakarrik dituzuelako [GitHub](https://github.com/)-en (dohainik, jakina). Geldituko ez bazenute, pare bat egunetan agortuko zenituzke. Zure codespace gelditzeko, Codespace atalean zure codespace-eko aukerak zabaldu eta "Stop codespace" hautatu:

    ![7a. Go to Codespaces](/images/GoToCodespaces.png "7a. Go to Codespaces")
   
    ![7b. Stop codespace](/images/StopCodespace.png "7b. Stop codespace")

8. Zure codespace berriro erabiltzeko, Codespace atalean zure codespace-eko izenean klikatu eta automatikoki martxan jarriko da. Lehen bezala, terminal leihoan hurrengo komando exekutatu:

    ```bash
    docker run --name easyatp -p 3000:3000 -d javieralvez/easyatp:2024
    ```

    ![8a. Start codespace](/images/StartCodespace.png "8a. Start codespace")

    ![8b. Re-exekute Docker Run Command](/images/DockerRunCommandAgain.png "8b. Re-exekute Docker Run Command")

9. Errore bat agertzen bazaizu, saia zaitez biltegia ezabatzen hurrengo komandoa erabiliz:

    ```bash
    docker container rm "biltegi-gakoa"
    ```

    non "biltegi-gakoa" errore-mezuan agertzen zaizu. Ondoren, "run" komandoa berriro exekutatu eta martxan jarriko da EasyATP:

    ![9a. Delete Docker Container](/images/DeleteDockerContainer.png "9a. Delete Docker Container")

    ![9b. Re-exekute Docker Run Command Again](/images/DockerRunCommandOnceAgain.png "9b. Re-exekute Docker Run Command Again")



