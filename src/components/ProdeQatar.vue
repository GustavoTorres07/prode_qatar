<template>

    <div class="container-fluid text-center">
        <h1 class="">
            Prode Qatar 2022
        </h1>

        <br>

        <div class="card border-primary centrar">
            <div class="card-header mb-3">Datos Personales</div>
            <div class="col-xs-2 mb-3">
                <label for="ex1">Apellido</label>
                <input class="form-control text-center" id="inputApellido" type="text">
                <br>
                <label for="ex1">Nombre</label>
                <input class="form-control text-center" id="inputNombre" type="text">
                <br>
                <label for="ex1">Telefono</label>
                <input class="form-control text-center" id="inputTelefono" type="number">
                <br>
                <button type="submit" class="btn btn-success">Guardar Prode</button>
            </div>
        </div>

        <br>

        <!-- Button trigger modal -->
        <button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#Modal1">
            LEER CONDICIONES GENERALES
        </button>
        <!-- Modal 1 -->
        <div class="modal fade" id="Modal1" tabindex="-1" aria-labelledby="ModalLabel" aria-hidden="true">
            <div class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-header">
                        <h5 class="modal-title text-danger" id="ModalLabel1">Condiciones Generales</h5>
                        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                    </div>
                    <div class="modal-body">

                        <p class="text-center">El objetivo del juego es poder realizar la mayor cantidad
                            de puntos. Teniendo chances todos los participantes de
                            acceder a los premios en juego.
                            ¿Como se obtienen los puntos?
                            Los participantes obtendrán sus puntos de acuerdo a las reglas.</p>

                    </div>
                    <div class="modal-footer">
                        <button type="button" class="btn btn-warning" data-bs-dismiss="modal">Cerrar</button>
                    </div>
                </div>
            </div>
        </div>

        <!-- Button trigger modal -->
        <button type="button" style="margin-left: 10px" class="btn btn-primary" data-bs-toggle="modal"
            data-bs-target="#Modal2">
            LEER REGLAS
        </button>
        <!-- Modal 2 -->
        <div class="modal fade" id="Modal2" tabindex="-1" aria-labelledby="exampleModalLabel2" aria-hidden="true">
            <div class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-header">
                        <h5 class="modal-title text-danger" id="ModalLabel2">Reglas</h5>
                        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                    </div>
                    <div class="modal-body">

                        <p class="text-center"> A)- Por cada acierto (en forma local, empate o
                            visitante) en los resultados de la primera fase se
                            obtendrán 3 puntos. (48 partidos por 3
                            puntos = 144 puntos en juego).
                            <br>B)- Por cada equipo acertado de los cuatro mejores,
                            se obtendrán 7 puntos. (Equipos en semi final 4 x 7
                            puntos = 28 puntos en juego).
                            <br>C)- Los participantes que acierten el equipo campeón
                            obtendrán 12 puntos.<br><br>
                            PUNTAJE MÁXIMO POSIBLE “184 PUNTOS”
                        </p>

                    </div>
                    <div class="modal-footer">
                        <button type="button" class="btn btn-warning" data-bs-dismiss="modal">Cerrar</button>
                    </div>
                </div>
            </div>
        </div>

        <!-- Button trigger modal -->
        <button type="button" style="margin-left: 10px" class="btn btn-primary" data-bs-toggle="modal"
            data-bs-target="#Modal3">
            LEER PREMIOS
        </button>
        <!-- Modal 3 -->
        <div class="modal fade" id="Modal3" tabindex="-1" aria-labelledby="ModalLabel3" aria-hidden="true">
            <div class="modal-dialog">
                <div class="modal-content">
                    <div class="modal-header">
                        <h5 class="modal-title text-danger" id="ModalLabel2"> Premios </h5>
                        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                    </div>
                    <div class="modal-body">

                        <p class="text-center">De existir empate en el primer puesto se repartirá la suma de
                            los premios ($20.000) en iguales cantidades entre los ganadores.
                            De existir un solo ganador (cobrara $15.000) y empate en el
                            segundo puesto, se repartirán el segundo premio ($5000) en
                            partes iguales.</p>

                    </div>
                    <div class="modal-footer">
                        <button type="button" class="btn btn-warning" data-bs-dismiss="modal">Cerrar</button>
                    </div>
                </div>
            </div>
        </div>

        <br>
        <br>

        <div class="col mb-4">
            <h2> Copa Mundial de la FIFA Qatar 2022 </h2>
        </div>

        <button type="button" class="btn btn-success" @click="mostrarpuntaje">
            <h3>Mostrar Puntaje</h3>
        </button><br><br>

        <span>
            <h3> TU PUNTAJE ES: {{ puntos }}</h3>
        </span>

        <br><br>

        <div class="row cards" style="width: auto; margin: auto auto;">

            <div class="col-lg-3">
                <div class="card tarjeta">
                    <div class="card-header bg-transparent"><b><h2> GRUPO A </h2></b></div>
                    <div class="card-body">
                        <div class="control-group">
                            <div class="controls">
                                <label class="radiobtn btn btn-secondary estilolabel" >
                                    <input type="radio" value="workTipe1" id="optionsRadios1" autocomplete="off"
                                        name="optionsRadios1">
                                    QATAR
                                </label>
                                <label class="radio btn btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe2" id="optionsRadios2" autocomplete="off"
                                        name="optionsRadios1">
                                    EMPATE
                                </label>
                                <label class="radio btn btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe3" id="optionsRadios3" name="optionsRadios1">
                                    ECUADOR
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe4" id="optionsRadios4" autocomplete="off"
                                        name="optionsRadios2">
                                    SENEGAL
                                </label>
                                <label class="radio btn btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe5" id="optionsRadios5" autocomplete="off"
                                        name="optionsRadios2">
                                    EMPATE
                                </label>
                                <label class="radio btn btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe6" id="optionsRadios6" name="optionsRadios2">
                                    PAISES BAJOS
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe7" id="optionsRadios7" autocomplete="off"
                                        name="optionsRadios3">
                                    QATAR 
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe8" id="optionsRadios8" autocomplete="off"
                                        name="optionsRadios3">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe9" id="optionsRadios9" name="optionsRadios3">
                                    SENEGAL
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe10" id="optionsRadios10" autocomplete="off"
                                        name="optionsRadios4">
                                    PAISES BAJOS
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe11" id="optionsRadios11" autocomplete="off"
                                        name="optionsRadios4">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe12" id="optionsRadios12" name="optionsRadios4">
                                    ECUADOR
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe13" id="optionsRadios13" autocomplete="off"
                                        name="optionsRadios5">
                                    ECUADOR
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe14" id="optionsRadios14" autocomplete="off"
                                        name="optionsRadios5">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe15" id="optionsRadios15" name="optionsRadios5">
                                    SENEGAL
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe16" id="optionsRadios16" autocomplete="off"
                                        name="optionsRadios6">
                                    PAISES BAJOS
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe17" id="optionsRadios17" autocomplete="off"
                                        name="optionsRadios6">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe18" id="optionsRadios18" name="optionsRadios6">
                                    QATAR
                                </label>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div class="col-lg-3">

                <div class="card tarjeta">
                    <div class="card-header bg-transparent"><h2> GRUPO B </h2></div>
                    <div class="card-body">
                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe19" id="optionsRadios19" autocomplete="off"
                                        name="optionsRadios7">
                                    INGLATERRA
                                </label>
                                <label class="radio btn btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe20" id="optionsRadios20" autocomplete="off"
                                        name="optionsRadios7">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe21" id="optionsRadios21" name="optionsRadios7">
                                    IRAN
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe22" id="optionsRadios22" autocomplete="off"
                                        name="optionsRadios8">
                                    ESTADOS UNIDOS
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe23" id="optionsRadios23" autocomplete="off"
                                        name="optionsRadios8">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe24" id="optionsRadios24" name="optionsRadios8">
                                    GALES
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe25" id="optionsRadios25" autocomplete="off"
                                        name="optionsRadios9">
                                    GALES
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe26" id="optionsRadios26" autocomplete="off"
                                        name="optionsRadios9">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe27" id="optionsRadios27" name="optionsRadios9">
                                    IRAN
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe28" id="optionsRadios28" autocomplete="off"
                                        name="optionsRadios10">
                                    INGLATERRA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe29" id="optionsRadios29" autocomplete="off"
                                        name="optionsRadios10">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe30" id="optionsRadios30" name="optionsRadios10">
                                    ESTADOS UNIDOS
                                </label>
                            </div>
                        </div>

                        <hr>


                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe31" id="optionsRadios31" autocomplete="off"
                                        name="optionsRadios11">
                                    IRAN
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe32" id="optionsRadios32" autocomplete="off"
                                        name="optionsRadios11">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe33" id="optionsRadios33" name="optionsRadios11">
                                    ESTADOS UNIDOS
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe34" id="optionsRadios34" autocomplete="off"
                                        name="optionsRadios12">
                                    GALES
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe35" id="optionsRadios35" autocomplete="off"
                                        name="optionsRadios12">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe36" id="optionsRadios36" name="optionsRadios12">
                                    INGLATERRA
                                </label>
                            </div>
                        </div>

                    </div>

                </div>

            </div>

            <div class="col mb-4">

                <div class="card tarjeta">
                    <div class="card-header bg-transparent"><H2> GRUPO C </H2></div>
                    <div class="card-body">
                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe37" id="optionsRadios37" autocomplete="off"
                                        name="optionsRadios13">
                                    ARGENTINA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe38" id="optionsRadios38" autocomplete="off"
                                        name="optionsRadios13">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe39" id="optionsRadios39" name="optionsRadios13">
                                    ARABIA SAUDITA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe40" id="optionsRadios40" autocomplete="off"
                                        name="optionsRadios14">
                                    MEXICO
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe41" id="optionsRadios41" autocomplete="off"
                                        name="optionsRadios14">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe42" id="optionsRadios42" name="optionsRadios14">
                                    POLONIA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe43" id="optionsRadios43" autocomplete="off"
                                        name="optionsRadios15">
                                    POLONIA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe44" id="optionsRadios44" autocomplete="off"
                                        name="optionsRadios15">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe45" id="optionsRadios45" name="optionsRadios15">
                                    ARABIA SAUDITA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe46" id="optionsRadios46" autocomplete="off"
                                        name="optionsRadios16">
                                    ARGENTINA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe47" id="optionsRadios47" autocomplete="off"
                                        name="optionsRadios16">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe48" id="optionsRadios48" name="optionsRadios16">
                                    MEXICO
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe49" id="optionsRadios49" autocomplete="off"
                                        name="optionsRadios17">
                                    POLONIA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe50" id="optionsRadios50" autocomplete="off"
                                        name="optionsRadios17">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe51" id="optionsRadios51" name="optionsRadios17">
                                    ARGENTINA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe52" id="optionsRadios52" autocomplete="off"
                                        name="optionsRadios18">
                                    ARABIA SAUDITA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe53" id="optionsRadios53" autocomplete="off"
                                        name="optionsRadios18">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe54" id="optionsRadios54" name="optionsRadios18">
                                    MEXICO
                                </label>
                            </div>
                        </div>

                    </div>

                </div>

            </div>





            <div class="col mb-4">
                <div class="card tarjeta">
                    <div class="card-header bg-transparent"><H2> GRUPO D </H2></div>
                    <div class="card-body">

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe55" id="optionsRadios55" autocomplete="off"
                                        name="optionsRadios19">
                                    DINAMARCA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe56" id="optionsRadios56" autocomplete="off"
                                        name="optionsRadios19">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe57" id="optionsRadios57" name="optionsRadios19">
                                    TUNEZ
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe58" id="optionsRadios58" autocomplete="off"
                                        name="optionsRadios20">
                                    FRANCIA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe59" id="optionsRadios59" autocomplete="off"
                                        name="optionsRadios20">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe60" id="optionsRadios60" name="optionsRadios20">
                                    AUSTRALIA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe61" id="optionsRadios61" autocomplete="off"
                                        name="optionsRadios21">
                                    TUNEZ
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe62" id="optionsRadios62" autocomplete="off"
                                        name="optionsRadios21">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe63" id="optionsRadios63" name="optionsRadios21">
                                    AUSTRALIA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe64" id="optionsRadios64" autocomplete="off"
                                        name="optionsRadios22">
                                    FRANCIA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe65" id="optionsRadios65" autocomplete="off"
                                        name="optionsRadios22">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe66" id="optionsRadios66" name="optionsRadios22">
                                    DINAMARCA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe67" id="optionsRadios67" autocomplete="off"
                                        name="optionsRadios23">
                                    AUSTRALIA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe68" id="optionsRadios68" autocomplete="off"
                                        name="optionsRadios23">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe69" id="optionsRadios69" name="optionsRadios23">
                                    DINAMARCA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe70" id="optionsRadios70" autocomplete="off"
                                        name="optionsRadios24">
                                    TUNEZ
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe71" id="optionsRadios71" autocomplete="off"
                                        name="optionsRadios24">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe72" id="optionsRadios72" name="optionsRadios24">
                                    FRANCIA
                                </label>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div class="row cards" style="width: auto; margin: auto auto;">

            <div class="col mb-4">
                <div class="card tarjeta">
                    <div class="card-header bg-transparent"><h2> GRUPO E </h2></div>
                    <div class="card-body">

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe73" id="optionsRadios73" autocomplete="off"
                                        name="optionsRadios25">
                                    ALEMANIA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe74" id="optionsRadios74" autocomplete="off"
                                        name="optionsRadios25">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe75" id="optionsRadios75" name="optionsRadios25">
                                    JAPON
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe76" id="optionsRadios76" autocomplete="off"
                                        name="optionsRadios26">
                                    ESPAÑA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe77" id="optionsRadios77" autocomplete="off"
                                        name="optionsRadios26">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe78" id="optionsRadios78" name="optionsRadios26">
                                    COSTA RICA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe79" id="optionsRadios79" autocomplete="off"
                                        name="optionsRadios27">
                                    JAPON
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe80" id="optionsRadios80" autocomplete="off"
                                        name="optionsRadios27">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe81" id="optionsRadios81" name="optionsRadios27">
                                    COSTA RICA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe82" id="optionsRadios82" autocomplete="off"
                                        name="optionsRadios28">
                                    ESPAÑA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe83" id="optionsRadios83" autocomplete="off"
                                        name="optionsRadios28">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe84" id="optionsRadios84" name="optionsRadios28">
                                    ALEMANIA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe85" id="optionsRadios85" autocomplete="off"
                                        name="optionsRadios29">
                                    COSTA RICA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe86" id="optionsRadios86" autocomplete="off"
                                        name="optionsRadios29">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe87" id="optionsRadios87" name="optionsRadios29">
                                    ALEMANIA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe88" id="optionsRadios88" autocomplete="off"
                                        name="optionsRadios30">
                                    JAPON
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe89" id="optionsRadios89" autocomplete="off"
                                        name="optionsRadios30">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe90" id="optionsRadios90" name="optionsRadios30">
                                    ESPAÑA
                                </label>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div class="col mb-4">
                <div class="card tarjeta">
                    <div class="card-header bg-transparent"><h2> GRUPO F </h2></div>
                    <div class="card-body">

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe91" id="optionsRadios91" autocomplete="off"
                                        name="optionsRadios31">
                                    MARRUECOS
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe92" id="optionsRadios92" autocomplete="off"
                                        name="optionsRadios31">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe93" id="optionsRadios93" name="optionsRadios31">
                                    CROACIA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe94" id="optionsRadios94" autocomplete="off"
                                        name="optionsRadios32">
                                    BELGICA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe95" id="optionsRadios95" autocomplete="off"
                                        name="optionsRadios32">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe96" id="optionsRadios96" name="optionsRadios32">
                                    CANADA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe97" id="optionsRadios97" autocomplete="off"
                                        name="optionsRadios33">
                                    BELGICA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe98" id="optionsRadios98" autocomplete="off"
                                        name="optionsRadios33">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe99" id="optionsRadios99" name="optionsRadios33">
                                    MARRUECOS
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe100" id="optionsRadios100" autocomplete="off"
                                        name="optionsRadios34">
                                    CROACIA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe101" id="optionsRadios101" autocomplete="off"
                                        name="optionsRadios34">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe102" id="optionsRadios102"
                                        name="optionsRadios34">
                                    CANADA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe103" id="optionsRadios103" autocomplete="off"
                                        name="optionsRadios35">
                                    CANADA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe104" id="optionsRadios104" autocomplete="off"
                                        name="optionsRadios35">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe105" id="optionsRadios105"
                                        name="optionsRadios35">
                                    MARRUECOS
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe106" id="optionsRadios106" autocomplete="off"
                                        name="optionsRadios36">
                                    CROACIA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe107" id="optionsRadios107" autocomplete="off"
                                        name="optionsRadios36">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe108" id="optionsRadios108"
                                        name="optionsRadios36">
                                    BELGICA
                                </label>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div class="col mb-4">
                <div class="card tarjeta">
                    <div class="card-header bg-transparent"><h2> GRUPO G </h2></div>
                    <div class="card-body">

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe109" id="optionsRadios109" autocomplete="off"
                                        name="optionsRadios37">
                                    SUIZA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe110" id="optionsRadios110" autocomplete="off"
                                        name="optionsRadios37">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe111" id="optionsRadios111"
                                        name="optionsRadios37">
                                    CAMERUN
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe112" id="optionsRadios112" autocomplete="off"
                                        name="optionsRadios38">
                                    BRASIL
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe113" id="optionsRadios113" autocomplete="off"
                                        name="optionsRadios38">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe114" id="optionsRadios114"
                                        name="optionsRadios38">
                                    SERBIA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe115" id="optionsRadios115" autocomplete="off"
                                        name="optionsRadios39">
                                    CAMERUN
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe116" id="optionsRadios116" autocomplete="off"
                                        name="optionsRadios39">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe117" id="optionsRadios117"
                                        name="optionsRadios39">
                                    SERBIA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe118" id="optionsRadios118" autocomplete="off"
                                        name="optionsRadios40">
                                    BRASIL
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe119" id="optionsRadios119" autocomplete="off"
                                        name="optionsRadios40">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe120" id="optionsRadios120"
                                        name="optionsRadios40">
                                    SUIZA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe121" id="optionsRadios121" autocomplete="off"
                                        name="optionsRadios41">
                                    CAMERUN
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe122" id="optionsRadios122" autocomplete="off"
                                        name="optionsRadios41">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe123" id="optionsRadios123"
                                        name="optionsRadios41">
                                    BRASIL
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe124" id="optionsRadios124" autocomplete="off"
                                        name="optionsRadios42">
                                    SERBIA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe125" id="optionsRadios125" autocomplete="off"
                                        name="optionsRadios42">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe126" id="optionsRadios126"
                                        name="optionsRadios42">
                                    SUIZA
                                </label>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div class="col mb-4">
                <div class="card tarjeta">
                    <div class="card-header bg-transparent"><h2> GRUPO H </h2></div>
                    <div class="card-body">

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe127" id="optionsRadios127" autocomplete="off"
                                        name="optionsRadios43">
                                    URUGUAY
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe128" id="optionsRadios128" autocomplete="off"
                                        name="optionsRadios43">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe129" id="optionsRadios129"
                                        name="optionsRadios43">
                                    COREA DEL SUR
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe130" id="optionsRadios130" autocomplete="off"
                                        name="optionsRadios44">
                                    PORTUGAL
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe131" id="optionsRadios131" autocomplete="off"
                                        name="optionsRadios44">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe132" id="optionsRadios132"
                                        name="optionsRadios44">
                                    GHANA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe133" id="optionsRadios133" autocomplete="off"
                                        name="optionsRadios45">
                                    COREA DEL SUR
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe134" id="optionsRadios134" autocomplete="off"
                                        name="optionsRadios45">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe135" id="optionsRadios135"
                                        name="optionsRadios45">
                                    GHANA
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe136" id="optionsRadios136" autocomplete="off"
                                        name="optionsRadios46">
                                    PORTUGAL
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe137" id="optionsRadios137" autocomplete="off"
                                        name="optionsRadios46">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe138" id="optionsRadios138"
                                        name="optionsRadios46">
                                    URUGUAY
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe139" id="optionsRadios139" autocomplete="off"
                                        name="optionsRadios47">
                                    GHANA
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe140" id="optionsRadios140" autocomplete="off"
                                        name="optionsRadios47">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe141" id="optionsRadios141"
                                        name="optionsRadios47">
                                    URUGUAY
                                </label>
                            </div>
                        </div>

                        <hr>

                        <div class="control-group">
                            <div class="controls">
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe142" id="optionsRadios142" autocomplete="off"
                                        name="optionsRadios48">
                                    COREA DEL SUR
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe143" id="optionsRadios143" autocomplete="off"
                                        name="optionsRadios48">
                                    EMPATE
                                </label>
                                <label class="radio btn btn-secondary estilolabel">
                                    <input type="radio" value="workTipe144" id="optionsRadios144"
                                        name="optionsRadios48">
                                    PORTUGAL
                                </label>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div class="container">

            <div class="row cards" style="width: auto; margin: auto auto;">

                <div class="col mb-4">
                    <div class="card tarjeta">
                        <div class="card-header bg-transparent"><h2> Cuartos de final </h2></div>
                        <div class="card-body">

                            <div class="control-group">
                                <div class="controls">
                                    <label class="radio btn btn-secondary estilolabel">
                                        <input type="radio" value="workTipe145" id="optionsRadios145" autocomplete="off"
                                            name="optionsRadios49">
                                        Vencedor 1°A o 2°B
                                    </label>
                                    <label class="radio btn btn-secondary estilolabel">
                                        <input type="radio" value="workTipe146" id="optionsRadios146"
                                            name="optionsRadios49">
                                        Vencedor 1°C o 2°D
                                    </label>
                                </div>
                            </div>

                            <hr>

                            <div class="control-group">
                                <div class="controls">
                                    <label class="radio btn btn-secondary estilolabel">
                                        <input type="radio" value="workTipe147" id="optionsRadios147" autocomplete="off"
                                            name="optionsRadios50">
                                            Vencedor 1°E o 2°F
                                    </label> 
                                    <label class="radio btn btn-secondary estilolabel">
                                        <input type="radio" value="workTipe148" id="optionsRadios148"
                                            name="optionsRadios50">
                                            Vencedor 1°G o 2°H
                                    </label>
                                </div>
                            </div>

                            <hr>

                            <div class="control-group">
                                <div class="controls">
                                    <label class="radio btn btn-secondary estilolabel">
                                        <input type="radio" value="workTipe149" id="optionsRadios149" autocomplete="off"
                                            name="optionsRadios51">
                                            Vencedor 1°B o 2°A
                                    </label>
                                    <label class="radio btn btn-secondary estilolabel">
                                        <input type="radio" value="workTipe150" id="optionsRadios150"
                                            name="optionsRadios51">
                                            Vencedor 1°D o 2°C
                                    </label>
                                </div>
                            </div>

                            <hr>

                            <div class="control-group">
                                <div class="controls">
                                    <label class="radio btn btn-secondary estilolabel">
                                        <input type="radio" value="workTipe151" id="optionsRadios151" autocomplete="off"
                                            name="optionsRadios52">
                                            Vencedor 1°F o 2°E
                                    </label>
                                    <label class="radio btn btn-secondary estilolabel">
                                        <input type="radio" value="workTipe152" id="optionsRadios152"
                                            name="optionsRadios52">
                                            Vencedor 1°H o 2°G
                                    </label>
                                </div>
                            </div>

                        </div>
                    </div>

                </div>


                <div class="col mb-4">
                    <div class="card tarjeta">
                        <div class="card-header bg-transparent"><h2> Final </h2></div>
                        <div class="card-body">

                            <div class="control-group">
                                <div class="controls">
                                    <label class="radio btn btn-secondary estilolabel">
                                        <input type="radio" value="workTipe153" id="optionsRadios153" autocomplete="off"
                                            name="optionsRadios53">
                                        FINALISTA 1
                                    </label>
                                    <label class="radio btn btn-secondary estilolabel">
                                        <input type="radio" value="workTipe154" id="optionsRadios154"
                                            name="optionsRadios53">
                                        FINALISTA 2
                                    </label>
                                </div>
                            </div>

                        </div>
                    </div>

                </div>

            </div>

        </div>

    </div>
    
</template>

<script>


export default {

    data() {
        return {

            puntos: 0


        }
    },

    methods: {
        
        mostrarpuntaje() {


            if (document.getElementById('optionsRadios1').checked) {

                this.puntos = 0;

            }
            if (document.getElementById('optionsRadios2').checked) {

                this.puntos = 0;
            }
            if (document.getElementById('optionsRadios3').checked) {

                this.puntos = 3;
            }
            if (document.getElementById('optionsRadios4').checked) {

                this.puntos += 0;
            }
            if (document.getElementById('optionsRadios5').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios6').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios7').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios8').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios9').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios10').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios11').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios12').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios13').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios14').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios15').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios16').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios17').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios18').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios19').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios20').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios21').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios22').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios23').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios24').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios25').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios26').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios27').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios28').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios29').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios30').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios31').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios32').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios33').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios34').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios35').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios36').checked) {

                this.puntos += 3
            }

            if (document.getElementById('optionsRadios37').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios38').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios39').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios40').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios41').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios42').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios43').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios44').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios45').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios46').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios47').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios48').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios49').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios50').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios51').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios52').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios53').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios54').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios55').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios56').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios57').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios58').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios59').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios60').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios61').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios62').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios63').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios64').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios65').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios66').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios67').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios68').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios69').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios70').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios71').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios72').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios73').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios74').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios75').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios76').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios77').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios78').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios79').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios80').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios81').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios82').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios83').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios84').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios85').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios86').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios87').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios88').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios89').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios90').checked) {

                this.puntos += 3
            }

            if (document.getElementById('optionsRadios91').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios92').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios93').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios94').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios95').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios96').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios97').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios98').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios99').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios100').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios101').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios102').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios103').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios104').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios105').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios106').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios107').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios108').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios109').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios110').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios111').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios112').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios113').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios114').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios115').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios116').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios117').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios118').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios119').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios120').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios121').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios122').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios123').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios124').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios125').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios126').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios127').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios128').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios129').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios130').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios131').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios132').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios133').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios134').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios135').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios136').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios137').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios138').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios139').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios140').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios141').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios142').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios143').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios144').checked) {

                this.puntos += 3
            }
            if (document.getElementById('optionsRadios145').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios146').checked) {

                this.puntos += 7
            }
            if (document.getElementById('optionsRadios147').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios148').checked) {

                this.puntos += 7
            }
            if (document.getElementById('optionsRadios149').checked) {

                this.puntos += 7
            }
            if (document.getElementById('optionsRadios150').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios151').checked) {

                this.puntos += 7
            }
            if (document.getElementById('optionsRadios152').checked) {

                this.puntos += 0
            }
            if (document.getElementById('optionsRadios153').checked) {

                this.puntos += 12
            }
            if (document.getElementById('optionsRadios154').checked) {

                this.puntos += 0
            }

            // alert(puntos);
        }

    }

};

</script>
  
<style scoped>

.tarjeta{
    border-radius: 8px;
    box-shadow: 0 2px 2px rgba(11, 11, 11, 0.5);
    background-color: #fffffc23;
    color: #030302;
    margin-bottom: 50px;
    position: relative;
    z-index: 1;
}

.estilolabel { 
text-decoration:none;
font-weight: 600;
font-size: 15px;
color:#333333;
padding-top:15px; 
padding-bottom:15px; 
/* padding-left:40px; 
padding-right:40px;  */
background-color:#FFD27D;
border-color: #d8d8d8;
border-width: 3px;
border-style: solid;

}
.add-margin {
    margin-right: 10px
}

.centrar {
    width: 250px;
    margin: auto
}
</style>