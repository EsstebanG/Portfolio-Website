/* Estilo general de la tabla */
table {
    width: 100%;
    border-collapse: collapse;
    margin-top: 1rem;
    font-family: 'Noto Sans', sans-serif;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

/* Encabezados */
table th {
    background-color: #dba4a4;
    color: #fff;
    text-align: left;
    padding: 12px;
    font-weight: bold;
    font-size: 1rem;
}

/* Filas de la tabla */
table td {
    padding: 12px;
    border-bottom: 1px solid #ddd;
}

/* Alternar colores en filas */
table tr:nth-child(even) {
    background-color: #f9f9f9;
}

/* Efecto hover */
table tr:hover {
    background-color: #ffe9e9;
    transition: background-color 0.3s ease;
}

/* Estilo para los enlaces */
table a {
    color: #c94f4f;
    text-decoration: none;
    font-weight: 600;
}

table a:hover {
    text-decoration: underline;
}

/* Responsive (pantallas pequeñas) */
@media (max-width: 600px) {
    table, thead, tbody, th, td, tr {
        display: block;
    }

    table thead {
        display: none;
    }

    table tr {
        margin-bottom: 1rem;
        border-bottom: 2px solid #ccc;
    }

    table td {
        padding-left: 50%;
        position: relative;
    }

    table td::before {
        position: absolute;
        left: 1rem;
        width: 45%;
        white-space: nowrap;
        font-weight: bold;
    }

    table td:nth-of-type(1)::before { content: "Project name"; }
    table td:nth-of-type(2)::before { content: "Technologies Used"; }
    table td:nth-of-type(3)::before { content: "Link"; }
}