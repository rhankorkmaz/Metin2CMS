<div id="top_content_server_2" class="top_content_server top_active_block">
                            <div id="cp_block_server" class="top_player_block_server_1">
                                <table class="top_pvp top_block">
                                    <tbody>
                                        <tr>
                                            <td>&nbsp;</td>
                                            <td class="td-header">Character</td>
                                            <td class="td-header">Cp</td>
                                        </tr>
                                        <?php  
                                        include("inc/db_ayar.php");
                                        $con = mysqli_connect("0.0.0.0", "root", "", "ts25_gamedb");
                                        $bul = mysqli_query($con, "select aName, aKillOtherTribe from avatarinfo order by aKillOtherTribe desc");
                                        $i = 0;
                                        while($goster = mysqli_fetch_array($bul, MYSQLI_ASSOC)){
                                            echo 
                                            "<tr>
                                            <td>".$goster["aName"]."</td>
                                            <td>&nbsp;</td>
                                            <td>".$goster["aKillOtherTribe"]."</td>
                                            </tr>";
                                            $i++;
                                            if($i == 5)
                                        break;
                                        }
                                        ?>
                                    </tbody>
                                </table>
                            </div>
                        </div>

Dude, to adapt it to other games.

I need a panel for my db table

We want to adapt;
Options are limited in cms panel
What can we do
