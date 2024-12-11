<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lost&Found - Documentación</title>
    <style>
        :root {
            --primary: #8C2B59;
            --primary-dark: #732C4D;
            --secondary: #A66F89;
            --light: #F2C9DC;
            --text-primary: #2c3e50;
            --bg-light: #f8f9fa;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif;
        }

        body {
            background-color: white;
            color: var(--text-primary);
            line-height: 1.7;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
        }

        .hero {
            background-color: var(--primary);
            padding: 4rem 0;
            margin-bottom: 3rem;
        }

        .hero-content {
            text-align: center;
            color: white;
        }

        .hero h1 {
            font-size: 3.5rem;
            font-weight: 300;
            margin-bottom: 1rem;
            letter-spacing: -0.5px;
        }

        .hero p {
            font-size: 1.25rem;
            max-width: 700px;
            margin: 0 auto;
            opacity: 0.9;
            font-weight: 300;
        }

        .main-content {
            padding: 2rem 0;
        }

        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin: 2rem 0 4rem 0;
        }

        .feature-card {
            background: var(--bg-light);
            border-radius: 4px;
            padding: 1.75rem;
            border: 1px solid #eee;
        }

        .feature-card h3 {
            color: var(--primary);
            margin-bottom: 1rem;
            font-size: 1.25rem;
            font-weight: 600;
        }

        .feature-card p {
            color: #666;
            font-size: 1rem;
            margin-bottom: 1rem;
        }

        .feature-card ul {
            list-style: none;
            margin-top: 1rem;
        }

        .feature-card ul li {
            color: #666;
            font-size: 0.95rem;
            margin-bottom: 0.5rem;
            padding-left: 1.5rem;
            position: relative;
        }

        .feature-card ul li::before {
            content: "•";
            color: var(--secondary);
            font-weight: bold;
            position: absolute;
            left: 0;
        }

        .documentation-section {
            margin: 4rem 0;
            text-align: center;
        }

        .documentation-section h2 {
            color: var(--primary-dark);
            margin-bottom: 2rem;
            font-weight: 400;
            font-size: 2rem;
        }

        .docs-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 2rem;
            margin-top: 2rem;
        }

        .doc-card {
            background: white;
            border: 1px solid #eee;
            border-radius: 4px;
            padding: 2rem;
            text-align: left;
            transition: transform 0.2s ease, box-shadow 0.2s ease;
        }

        .doc-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
        }

        .doc-card h4 {
            color: var(--primary);
            margin-bottom: 1rem;
            font-size: 1.3rem;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .doc-card h4 svg {
            width: 24px;
            height: 24px;
        }

        .doc-card p {
            color: #666;
            font-size: 1rem;
            margin-bottom: 1.5rem;
            line-height: 1.6;
        }

        .doc-card ul {
            list-style: none;
            margin: 1rem 0;
        }

        .doc-card ul li {
            color: #666;
            font-size: 0.95rem;
            margin-bottom: 0.75rem;
            padding-left: 1.5rem;
            position: relative;
        }

        .doc-card ul li::before {
            content: "✓";
            color: var(--secondary);
            position: absolute;
            left: 0;
        }

        .doc-link {
            color: var(--secondary);
            text-decoration: none;
            font-size: 1rem;
            display: inline-flex;
            align-items: center;
            padding: 0.5rem 1rem;
            border: 1px solid var(--secondary);
            border-radius: 4px;
            margin-top: 1rem;
            transition: all 0.2s ease;
        }

        .doc-link:hover {
            background: var(--secondary);
            color: white;
        }

        .doc-link svg {
            width: 16px;
            height: 16px;
            margin-left: 8px;
        }

        @media (max-width: 768px) {
            .docs-grid {
                grid-template-columns: 1fr;
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .container {
                padding: 0 1rem;
            }
        }
    </style>
</head>
<body>
    <div class="hero">
        <div class="container hero-content">
            <h1>Lost&Found</h1>
            <p>Sistema integral para la gestión y recuperación de objetos perdidos</p>
        </div>
    </div>

    <div class="container main-content">
        <div class="features-grid">
            <div class="feature-card">
                <h3>Gestión Eficiente</h3>
                <p>Sistema completo para el registro y seguimiento de objetos perdidos con flujo de trabajo optimizado.</p>
                <ul>
                    <li>Registro detallado de objetos con fotografías</li>
                    <li>Seguimiento en tiempo real del estado</li>
                    <li>Notificaciones automáticas</li>
                </ul>
            </div>
            <div class="feature-card">
                <h3>Multiplataforma</h3>
                <p>Aplicación móvil desarrollada en Flutter, garantizando accesibilidad y experiencia consistente.</p>
                <ul>
                    <li>Disponible para Web y Android</li>
                    <li>Interfaz intuitiva y moderna</li>
                    <li>Sincronización en tiempo real</li>
                </ul>
            </div>
            <div class="feature-card">
                <h3>Seguridad y Privacidad</h3>
                <p>Implementación de medidas de seguridad robustas para proteger la información.</p>
                <ul>
                    <li>Autenticación segura de usuarios</li>
                    <li>Encriptación de datos sensibles</li>
                    <li>Control de acceso</li>
                </ul>
            </div>
        </div>

        <div class="documentation-section">
            <h2>Documentación</h2>
            <div class="docs-grid">
                <div class="doc-card">
                    <h4>
                        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                            <path d="M12 12v.01M12 16v.01M12 8v.01M21 12c0 4.97-4.03 9-9 9s-9-4.03-9-9 4.03-9 9-9 9 4.03 9 9z"/>
                        </svg>
                        Manual de Usuario
                    </h4>
                    <p>Guía completa y detallada para usuarios finales sobre todas las funcionalidades de la aplicación Lost&Found.</p>
                    <ul>
                        <li>Proceso de registro y configuración inicial</li>
                        <li>Guía de registro de objetos perdidos</li>
                        <li>Proceso de reclamación de objetos</li>
                    </ul>
                    <a href="manual_usuario" class="doc-link">
                        Ver manual
                        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                            <path d="M5 12h14M12 5l7 7-7 7"/>
                        </svg>
                    </a>
                </div>
                <div class="doc-card">
                    <h4>
                        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                            <path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/>
                            <path d="M14 2v6h6M16 13H8M16 17H8M10 9H8"/>
                        </svg>
                        Informe General
                    </h4>
                    <p>Documentación detallada sobre la arquitectura, componentes y funcionalidades del sistema Lost&Found.</p>
                    <ul>
                        <li>Visión general del proyecto</li>
                        <li>Metodologias Usadas</li>
                        <li>Flujos de trabajo principales</li>
                        <li>Herramientas de Desarrollo</li>
                    </ul>
                    <a href="informe_general" class="doc-link">
                        Ver informe
                        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                            <path d="M5 12h14M12 5l7 7-7 7"/>
                        </svg>
                    </a>
                </div>
            </div>
        </div>
    </div>
</body>
</html>