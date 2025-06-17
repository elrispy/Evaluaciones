<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Evaluación de Puestos</title>
  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  <!-- React y ReactDOM CDN -->
  <script src="https://cdn.jsdelivr.net/npm/react@18.2.0/umd/react.production.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/react-dom@18.2.0/umd/react-dom.production.min.js"></script>
  <!-- Babel CDN para JSX -->
  <script src="https://cdn.jsdelivr.net/npm/@babel/standalone@7.20.15/babel.min.js"></script>
  <!-- Chart.js CDN -->
  <script src="https://cdn.jsdelivr.net/npm/chart.js@4.4.0/dist/chart.umd.min.js"></script>
  <!-- FileSaver.js CDN para exportar CSV -->
  <script src="https://cdn.jsdelivr.net/npm/file-saver@2.0.5/dist/FileSaver.min.js"></script>
</head>
<body class="bg-gray-100 min-h-screen flex items-center justify-center">
  <div id="root"></div>
  <script type="text/babel">
    const { useState, useEffect } = React;

    // Definición del cuestionario
    const questions = [
      {
        section: "Complejidad de Tareas",
        items: [
          {
            text: "¿Qué nivel de especialización requieren las tareas principales del colaborador?",
            options: [
              "Tareas rutinarias, sin requerimientos de especialización (1)",
              "Tareas que requieren conocimientos moderados o capacitación específica (2)",
              "Tareas altamente especializadas, con necesidad de experiencia avanzada (3)",
              "Tareas estratégicas que demandan expertise único o innovador (4)"
            ]
          },
          {
            text: "¿Cómo se estructuran las tareas asignadas al colaborador?",
            options: [
              "Totalmente estructuradas, con instrucciones detalladas (1)",
              "Parcialmente estructuradas, requieren cierta iniciativa (2)",
              "Mayormente no estructuradas, necesitan planificación independiente (3)",
              "Define procesos o estructuras para otros (4)"
            ]
          },
          {
            text: "¿Qué nivel de análisis o resolución de problemas implican las tareas?",
            options: [
              "Resolución de problemas simples y repetitivos (1)",
              "Resolución de problemas moderados con guías existentes (2)",
              "Resolución de problemas complejos con soluciones creativas (3)",
              "Diseño de soluciones innovadoras que establecen precedentes (4)"
            ]
          }
        ]
      },
      {
        section: "Toma de Decisiones",
        items: [
          {
            text: "¿Qué nivel de autonomía tiene el colaborador en la toma de decisiones?",
            options: [
              "Decisiones completamente guiadas por superiores (1)",
              "Decisiones operativas con supervisión cercana (2)",
              "Decisiones tácticas con autonomía moderada (3)",
              "Decisiones estratégicas con alta autonomía (4)"
            ]
          },
          {
            text: "¿Qué tipo de consecuencias tienen las decisiones del colaborador?",
            options: [
              "Impacto limitado, errores fácilmente corregibles (1)",
              "Impacto moderado en el equipo o proyecto (2)",
              "Impacto significativo en el área o departamento (3)",
              "Impacto crítico en la organización o clientes externos (4)"
            ]
          },
          {
            text: "¿Cómo se gestionan los riesgos asociados a las decisiones del colaborador?",
            options: [
              "Requiere aprobación constante para minimizar riesgos (1)",
              "Gestiona riesgos menores con supervisión (2)",
              "Gestiona riesgos moderados de forma autónoma (3)",
              "Anticipa y mitiga riesgos estratégicos (4)"
            ]
          }
        ]
      },
      {
        section: "Impacto Organizacional",
        items: [
          {
            text: "¿Cómo contribuyen las acciones del colaborador a los objetivos del negocio?",
            options: [
              "Soporte operativo con impacto indirecto (1)",
              "Contribución directa a metas del equipo (2)",
              "Influencia en metas del área o departamento (3)",
              "Definición de metas estratégicas organizacionales (4)"
            ]
          },
          {
            text: "¿Qué alcance tienen los resultados del trabajo del colaborador?",
            options: [
              "Alcance individual o de equipo pequeño (1)",
              "Alcance departamental (2)",
              "Alcance interdepartamental o multifuncional (3)",
              "Alcance organizacional o impacto externo (4)"
            ]
          },
          {
            text: "¿Qué nivel de innovación aportan las acciones del colaborador?",
            options: [
              "Ejecuta procesos establecidos sin cambios (1)",
              "Propone mejoras incrementales (2)",
              "Implementa soluciones innovadoras en su área (3)",
              "Lidera iniciativas transformadoras a nivel organizacional (4)"
            ]
          }
        ]
      },
      {
        section: "Competencias Técnicas",
        items: [
          {
            text: "¿Qué nivel de dominio tiene el colaborador en las herramientas o procesos del puesto?",
            options: [
              "Básico, requiere capacitación o guía constante (1)",
              "Intermedio, autónomo con errores ocasionales (2)",
              "Avanzado, resuelve problemas complejos (3)",
              "Experto, referente técnico para otros (4)"
            ]
          },
          {
            text: "¿Cómo aplica el colaborador sus conocimientos técnicos?",
            options: [
              "Ejecuta tareas técnicas definidas (1)",
              "Resuelve problemas técnicos moderados (2)",
              "Diseña soluciones técnicas innovadoras (3)",
              "Establece estándares técnicos o metodologías (4)"
            ]
          },
          {
            text: "¿Qué nivel de adaptabilidad tiene ante nuevas herramientas o procesos?",
            options: [
              "Resiste o requiere apoyo para adaptarse (1)",
              "Se adapta con capacitación moderada (2)",
              "Se adapta rápidamente de forma autónoma (3)",
              "Lidera la adopción de nuevas herramientas/procesos (4)"
            ]
          }
        ]
      },
      {
        section: "Competencias de Liderazgo",
        items: [
          {
            text: "¿Qué nivel de liderazgo ejerce el colaborador?",
            options: [
              "Sin responsabilidades de liderazgo, sigue instrucciones (1)",
              "Liderazgo ocasional bajo supervisión (2)",
              "Lidera equipos o proyectos con autonomía (3)",
              "Mentoriza y desarrolla otros líderes (4)"
            ]
          },
          {
            text: "¿Cómo influye el colaborador en el desempeño del equipo?",
            options: [
              "Sin influencia directa en otros (1)",
              "Motiva al equipo en tareas específicas (2)",
              "Inspira y alinea al equipo hacia metas comunes (3)",
              "Transforma la cultura o dinámica del equipo (4)"
            ]
          },
          {
            text: "¿Cómo gestiona el colaborador los conflictos dentro del equipo?",
            options: [
              "Evita o requiere apoyo para resolver conflictos (1)",
              "Resuelve conflictos menores con guía (2)",
              "Resuelve conflictos complejos de forma autónoma (3)",
              "Previene conflictos y fomenta colaboración (4)"
            ]
          }
        ]
      },
      {
        section: "Gestión de Stakeholders",
        items: [
          {
            text: "¿Cómo se comunica el colaborador con clientes internos o externos?",
            options: [
              "Comunicación básica, necesita apoyo constante (1)",
              "Comunicación clara y autónoma (2)",
              "Comunicación efectiva, resuelve conflictos (3)",
              "Comunicación estratégica, genera alianzas (4)"
            ]
          },
          {
            text: "¿Qué nivel de colaboración mantiene con otros equipos o áreas?",
            options: [
              "Colaboración limitada, centrada en su rol (1)",
              "Colabora activamente dentro de su área (2)",
              "Facilita colaboración interdepartamental (3)",
              "Lidera iniciativas de colaboración estratégica (4)"
            ]
          },
          {
            text: "¿Cómo gestiona el colaborador las expectativas de stakeholders?",
            options: [
              "Requiere guía para responder a expectativas (1)",
              "Responde adecuadamente con supervisión (2)",
              "Gestiona expectativas de forma proactiva (3)",
              "Anticipa y supera expectativas estratégicamente (4)"
            ]
          }
        ]
      }
    ];

    // Componente para una pregunta
    function Question({ index, text, options, onChange }) {
      return (
        <div className="mb-4">
          <p className="text-lg font-medium">{index + 1}. {text}</p>
          {options.map((option, i) => (
            <label key={i} className="block">
              <input
                type="radio"
                name={`question-${index}`}
                value={i + 1}
                onChange={(e) => onChange(index, parseInt(e.target.value))}
                className="mr-2"
              />
              {option}
            </label>
          ))}
        </div>
      );
    }

    // Componente principal
    function App() {
      const [employeeName, setEmployeeName] = useState("");
      const [scores, setScores] = useState(Array(18).fill(null));
      const [submitted, setSubmitted] = useState(false);
      const [chartInstance, setChartInstance] = useState(null);

      // Calcular puntaje total
      const totalScore = scores.reduce((sum, score) => sum + (score || 0), 0);

      // Determinar puesto
      const getPosition = (score) => {
        if (score >= 63) return "Líder/Jefe";
        if (score >= 48) return "Responsable/Coordinador";
        if (score >= 33) return "Analista";
        if (score >= 18) return "Asistente";
        return "No clasificado";
      };

      // Manejar cambio en las respuestas
      const handleScoreChange = (index, value) => {
        const newScores = [...scores];
        newScores[index] = value;
        setScores(newScores);
      };

      // Validar formulario
      const isFormComplete = scores.every(score => score !== null);

      // Generar datos para el gráfico
      const getChartData = () => {
        const dimensionScores = [];
        for (let i = 0; i < 6; i++) {
          const start = i * 3;
          const dimensionScore = scores.slice(start, start + 3).reduce((sum, s) => sum + (s || 0), 0);
          dimensionScores.push(dimensionScore);
        }
        return {
          labels: ["Complejidad", "Decisiones", "Impacto", "Técnicas", "Liderazgo", "Stakeholders"],
          datasets: [{
            label: "Puntaje por Dimensión",
            data: dimensionScores,
            backgroundColor: ["#36A2EB", "#FF6384", "#4BC0C0", "#FFCE56", "#9966FF", "#FF9F40"],
            borderColor: ["#2A80B9", "#CC4B37", "#3A9D9D", "#D4A017", "#7A52CC", "#D47F00"],
            borderWidth: 1
          }]
        };
      };

      // Crear gráfico
      useEffect(() => {
        if (submitted && isFormComplete) {
          const ctx = document.getElementById("resultsChart").getContext("2d");
          if (chartInstance) chartInstance.destroy();
          const newChart = new Chart(ctx, {
            type: "bar",
            data: getChartData(),
            options: {
              scales: {
                y: { beginAtZero: true, max: 12 }
              }
            }
          });
          setChartInstance(newChart);
        }
      }, [submitted, scores]);

      // Exportar a CSV
      const exportToCSV = () => {
        const headers = ["Colaborador", ...questions.flatMap(q => q.items.map((_, i) => `Pregunta ${q.items.indexOf(_) + 1 + questions.indexOf(q) * 3}`)), "Puntaje Total", "Puesto"];
        const row = [employeeName, ...scores, totalScore, getPosition(totalScore)];
        const csvContent = [headers, row].map(row => row.join(",")).join("\n");
        const blob = new Blob([csvContent], { type: "text/csv;charset=utf-8;" });
        saveAs(blob, `evaluacion_${employeeName || "colaborador"}.csv`);
      };

      // Manejar envío
      const handleSubmit = () => {
        if (isFormComplete && employeeName) {
          setSubmitted(true);
        } else {
          alert("Por favor, complete todas las preguntas y el nombre del colaborador.");
        }
      };

      return (
        <div className="max-w-4xl mx-auto p-6 bg-white rounded-lg shadow-md">
          <h1 className="text-2xl font-bold mb-6 text-center">Evaluación de Puestos</h1>
          <div className="mb-4">
            <label className="block text-lg font-medium mb-2">Nombre del Colaborador</label>
            <input
              type="text"
              value={employeeName}
              onChange={(e) => setEmployeeName(e.target.value)}
              className="w-full p-2 border rounded"
              placeholder="Ingrese el nombre"
            />
          </div>
          {questions.map((section, sectionIndex) => (
            <div key={sectionIndex} className="mb-8">
              <h2 className="text-xl font-semibold mb-4">{section.section}</h2>
              {section.items.map((question, qIndex) => (
                <Question
                  key={qIndex}
                  index={sectionIndex * 3 + qIndex}
                  text={question.text}
                  options={question.options}
                  onChange={handleScoreChange}
                />
              ))}
            </div>
          ))}
          <button
            onClick={handleSubmit}
            className="w-full bg-blue-600 text-white p-3 rounded hover:bg-blue-700 disabled:bg-gray-400"
            disabled={!employeeName || !isFormComplete}
          >
            Calcular Resultado
          </button>
          {submitted && isFormComplete && (
            <div className="mt-8">
              <h2 className="text-xl font-semibold mb-4">Resultados</h2>
              <p className="text-lg">Puntaje Total: {totalScore}</p>
              <p className="text-lg">Puesto Asignado: {getPosition(totalScore)}</p>
              <canvas id="resultsChart" className="mt-4"></canvas>
              <button
                onClick={exportToCSV}
                className="mt-4 bg-green-600 text-white p-3 rounded hover:bg-green-700"
              >
                Descargar Resultados (CSV)
              </button>
            </div>
          )}
        </div>
      );
    }

    // Renderizar la aplicación
    const root = ReactDOM.createRoot(document.getElementById("root"));
    root.render(<App />);
  </script>
</body>
</html>
