<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>+Vida - Servicios Médicos</title>
  <link rel="stylesheet" href="estilos.css" />
  <style>
    .modal {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: rgba(0, 0, 0, 0.5);
      display: flex; align-items: center; justify-content: center;
      z-index: 1000;
    }
    .modal-content {
      background: white;
      padding: 20px;
      border-radius: 8px;
      max-width: 500px;
      width: 90%;
      box-shadow: 0 2px 10px rgba(0,0,0,0.3);
    }
    .hidden {
      display: none;
    }
    label {
      display: block;
      margin-top: 10px;
    }
    input, select {
      width: 100%;
      padding: 8px;
      margin-top: 4px;
    }
  </style>
</head>
<body>
  <header>
    <div class="logo-titulo">
      <img src="logo-vida.png" alt="Logo +Vida" class="logo" />
    </div>
    <p class="slogan">Tu salud y tu tiempo son valiosos para nosotros. Con +Vida no hay deducibles, pagos extras ni trámites engorrosos.</p>
  </header>

  <nav class="navbar">
    <ul class="menu">
      <li><a href="#servicios">Servicios</a>
        <ul class="submenu">
          <li><a href="#consultas">Consultas y Urgencias</a></li>
          <li><a href="#estudios">Estudios Incluidos</a></li>
          <li><a href="#terapias">Terapias Físicas</a></li>
        </ul>
      </li>
      <li><a href="#precios">Precios</a>
        <ul class="submenu">
          <li><a href="#mensual">Mensual</a></li>
          <li><a href="#trimestral">Trimestral</a></li>
          <li><a href="#semestral">Semestral</a></li>
          <li><a href="#premium">Membresía Premium</a></li>
        </ul>
      </li>
      <li><a href="#procedimiento">Acceso</a></li>
      <li><a href="#no-incluye">No Incluye</a></li>
      <li><a href="#responsabilidad">Responsabilidad</a></li>
      <li><a href="#confidencialidad">Privacidad</a></li>
    </ul>
  </nav>

  <main>
    <section id="servicios" class="info">
      <h2>1. Servicios Incluidos</h2>
      <ul>
        <li>Consulta o urgencia mensual en Star Médica o San Ángel Inn.</li>
        <li>Estudios:
          <ul>
            <li>Hemograma completo</li>
            <li>Química sanguínea</li>
            <li>Examen general de orina</li>
            <li>Rayos X</li>
            <li>Electrocardiograma</li>
            <li>Pruebas COVID/influenza (con indicación médica)</li>
            <li>Coproparasitoscópico</li>
            <li>Determinación de grupo sanguíneo</li>
          </ul>
        </li>
        <li>3 terapias físicas mensuales con indicación médica.</li>
        <li>Tarjeta personalizada para acceso a hospitales afiliados.</li>
        <li>Urgencias menores: heridas abiertas, fracturas simples, estudios mencionados.</li>
      </ul>
      <p><strong>Importante:</strong> Urgencias mayores se canalizan a IMSS o seguro privado.</p>
    </section>

    <section id="precios" class="info">
      <h2>2. Precios y Beneficios</h2>
      <ul>
        <li id="mensual"><strong>Mensual:</strong> $1,199 MXN - prueba COVID/influenza con indicación médica.</li>
        <li id="trimestral"><strong>Trimestral:</strong> $3,600 MXN
          <ul>
            <li>Vacuna a elegir</li>
            <li>Prueba adicional para familiar</li>
            <li>Familiar a mitad de precio</li>
            <li>1 mes gratis si no se usa el servicio</li>
          </ul>
        </li>
        <li id="semestral"><strong>Semestral:</strong> $7,200 MXN
          <ul>
            <li>1 ambulancia en el periodo</li>
            <li>2 familiares a mitad de precio</li>
            <li>Vacuna o prueba extra</li>
            <li>2 meses adicionales si no se usa</li>
          </ul>
        </li>
        <li id="premium"><strong>Membresía Premium:</strong> $2,200 MXN mensuales - cualquier hospital privado dentro de CDMX o área metropolitana.</li>
      </ul>
    </section>

    <section id="procedimiento" class="info">
      <h2>3. Procedimiento para Acceder al Servicio</h2>
      <ul>
        <li>Urgencias: llamar al número de la tarjeta, dar datos personales y hospital.</li>
        <li>Consultas: llamar con 1 día de anticipación y coordinar cita.</li>
        <li>Presentar identificación y tarjeta de membresía.</li>
      </ul>
    </section>

    <section id="no-incluye" class="info">
      <h2>4. Servicios No Incluidos</h2>
      <ul>
        <li>Resonancias, tomografías, estudios avanzados</li>
        <li>Cirugías o enfermedades graves</li>
        <li>Reembolsos o deducibles</li>
        <li>Hospitales no afiliados (excepto premium)</li>
        <li>No se incluyen medicamentos</li>
      </ul>
    </section>

    <section id="responsabilidad" class="info">
      <h2>5. Limitación de Responsabilidad</h2>
      <p>+Vida es intermediario. No garantiza tiempos de espera ni decisiones médicas de hospitales.</p>
    </section>

    <section id="confidencialidad" class="info">
      <h2>6. Confidencialidad de Datos</h2>
      <p>Los datos del cliente se protegen conforme a la ley y se usan solo para fines administrativos.</p>
    </section>

    <section id="registro">
      <h2>Registro del Paciente</h2>
      <form id="registro-form">
        <label for="nombre-completo">Nombre Completo:</label>
        <input type="text" id="nombre-completo" required />

        <label for="fecha-nacimiento">Fecha de Nacimiento:</label>
        <input type="date" id="fecha-nacimiento" required />

        <label for="enfermedades-cronicas">Enfermedades Crónicas:</label>
        <textarea id="enfermedades-cronicas" rows="4"></textarea>

        <label for="telefono">Número de Contacto:</label>
        <input type="tel" id="telefono" required />

        <label for="email">Correo Electrónico:</label>
        <input type="email" id="email" required />

        <label for="comentarios">Comentarios Adicionales:</label>
        <textarea id="comentarios" rows="4"></textarea>

        <button type="submit">Registrar</button>
        <button type="button" id="btnAbrirContrato">Pagar</button>
      </form>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 +Vida. Todos los derechos reservados.</p>
  </footer>

  <!-- Modal Contrato -->
  <div id="modalContrato" class="modal hidden">
    <div class="modal-content">
      <h2>Contrato de Servicios Médicos +Vida</h2>
      <div style="max-height: 200px; overflow-y: auto; border: 1px solid #ccc; padding: 10px;">
        <p><strong>1. Servicios Incluidos:</strong> Una consulta o urgencia médica mensual en hospital privado...</p>
        <p><strong>Renovación automática:</strong> La membresía se renovará automáticamente al finalizar el periodo...</p>
        <!-- Más cláusulas aquí -->
      </div>
      <label><input type="checkbox" id="aceptoContrato" /> He leído y acepto los términos y condiciones.</label>
      <br><br>
      <button id="btnConfirmarPago" disabled>Continuar al Pago</button>
      <button id="btnCerrarContrato">Cancelar</button>
    </div>
  </div>

  <!-- Modal Pago -->
  <div id="modalPago" class="modal hidden">
    <div class="modal-content">
      <h2>Datos de Pago</h2>
      <label>Número de Tarjeta:</label>
      <input type="text" maxlength="16" placeholder="XXXX XXXX XXXX XXXX" />
      <label>Fecha de Vencimiento:</label>
      <input type="text" placeholder="MM/AA" />
      <label>CVV:</label>
      <input type="text" maxlength="4" placeholder="XXX" />
      <label>Nombre en la Tarjeta:</label>
      <input type="text" placeholder="Nombre completo" />
      <label>Selecciona tu paquete:</label>
      <select>
        <option value="mensual">Mensual - $1,199 MXN</option>
        <option value="trimestral">Trimestral - $3,600 MXN</option>
        <option value="semestral">Semestral - $7,200 MXN</option>
        <option value="premium">Premium - $2,200 MXN</option>
      </select>
      <br><br>
      <button onclick="finalizarPago()">Finalizar Pago</button>
      <button onclick="cerrarPago()">Cancelar</button>
    </div>
  </div>

  <script>
    const btnAbrirContrato = document.getElementById('btnAbrirContrato');
    const modalContrato = document.getElementById('modalContrato');
    const btnCerrarContrato = document.getElementById('btnCerrarContrato');
    const checkboxAcepto = document.getElementById('aceptoContrato');
    const btnConfirmarPago = document.getElementById('btnConfirmarPago');

    const modalPago = document.getElementById('modalPago');

    btnAbrirContrato.addEventListener('click', () => {
      modalContrato.classList.remove('hidden');
    });

    btnCerrarContrato.addEventListener('click', () => {
      modalContrato.classList.add('hidden');
      checkboxAcepto.checked = false;
      btnConfirmarPago.disabled = true;
    });

    checkboxAcepto.addEventListener('change', () => {
      btnConfirmarPago.disabled = !checkboxAcepto.checked;
    });

    btnConfirmarPago.addEventListener('click', () => {
      modalContrato.classList.add('hidden');
      modalPago.classList.remove('hidden');
    });

    function cerrarPago() {
      modalPago.classList.add('hidden');
    }

    function finalizarPago() {
      alert('Pago realizado con éxito. ¡Gracias por unirte a +Vida!');
      modalPago.classList.add('hidden');
    }
  </script>
</body>
</html>

