<div id="contact" class="contact">
    <div class="section secondary-section">
        <div class="container">
            <div class="title">
                <h1>Contactanos</h1>
                <p>Envianos un mensaje, estaremos felices de conocer tu empresa y crecer juntos.</p>
            </div>
        </div>
        <div class="map-wrapper">
            <div class="map-canvas" id="map-canvas">Cargando Mapa...</div>
            <div class="container">
                <div class="row-fluid">
                    <div class="span5 contact-form centered">
                        <h3>contacto</h3>
                        <div id="successSend" class="alert alert-success invisible">
                            <strong>Bien Hecho!</strong>Tu mensaje se a enviado exitosamente</div>
                        <div id="errorSend" class="alert alert-error invisible">ha ocurrido un error, intentelo de nuevo.</div>
                        <form id="contact-form" action="php/mail.php">
                            <div class="control-group">
                                <div class="controls">
                                    <input class="span12" type="text" id="name" name="name" placeholder="* Nombre..." />
                                    <div class="error left-align" id="err-name">Ingresa tu nombre.</div>
                                </div>
                            </div>
                            <div class="control-group">
                                <div class="controls">
                                    <input class="span12" type="email" name="email" id="email" placeholder="* Correo Electronico..." />
                                    <div class="error left-align" id="err-email">Ingresa tu correo electronico.</div>
                                </div>
                            </div>
                            <div class="control-group">
                                <div class="controls">
                                    <textarea class="span12" name="comment" id="comment" placeholder="* Comentario..."></textarea>
                                    <div class="error left-align" id="err-comment">Ingresa tu comentario.</div>
                                </div>
                            </div>
                            <div class="control-group">
                                <div class="controls">
                                    <button id="send-mail" class="message-btn">Enviar mensaje</button>
                                </div>
                            </div>
                        </form>
                    </div>
                </div>
            </div>
        </div>
        <div class="container">
            <div class="span9 center contact-info">
                <p>123 Fifth Avenue, 12th,Belgrade,SRB 11000</p>
                <p class="info-mail">info@qalaub.es</p>
                <p>+34 647 42 36 29</p>
                <p>+1 551 274 9097</p>
                <div class="title">
                    <h3>nuestras redes sociales</h3>
                </div>
            </div>
            <div class="row-fluid centered">
                <ul class="social">
                    <li>
                        <a href="">
                            <span class="icon-facebook-circled"></span>
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <span class="icon-twitter-circled"></span>
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <span class="icon-linkedin-circled"></span>
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <span class="icon-pinterest-circled"></span>
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <span class="icon-dribbble-circled"></span>
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <span class="icon-gplus-circled"></span>
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</div>