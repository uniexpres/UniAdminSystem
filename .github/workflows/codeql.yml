// Autor: 1006501633 - MICHELLE TATIANA VARGAS PACHECO

import java.util.ArrayList;
import java.util.List;

// Clase base Persona
abstract class Persona {
    protected String id;
    protected String nombre;

    public Persona(String id, String nombre) {
        this.id = id;
        this.nombre = nombre;
    }

    public String getNombre() {
        return nombre;
    }

    public String getId() {
        return id;
    }
}

// Clase Profesor que hereda de Persona
class Profesor extends Persona {
    private double salario;
    private List<Curso> cursos;

    public Profesor(String id, String nombre, double salario) {
        super(id, nombre);
        this.salario = salario;
        this.cursos = new ArrayList<>();
    }

    public void asignarCurso(Curso curso) {
        cursos.add(curso);
    }

    public List<Curso> consultarCursos() {
        return cursos;
    }

    public double getSalario() {
        return salario;
    }
}

// Clase Estudiante que hereda de Persona
class Estudiante extends Persona {
    private String direccion;
    private List<Curso> cursosInscritos;

    public Estudiante(String id, String nombre, String direccion) {
        super(id, nombre);
        this.direccion = direccion;
        this.cursosInscritos = new ArrayList<>();
    }

    public void inscribirseCurso(Curso curso) {
        cursosInscritos.add(curso);
    }

    public List<Curso> consultarCursosInscritos() {
        return cursosInscritos;
    }
}

// Clase Curso
class Curso {
    private String codigo;
    private String nombre;
    private Departamento departamento;

    public Curso(String codigo, String nombre, Departamento departamento) {
        this.codigo = codigo;
        this.nombre = nombre;
        this.departamento = departamento;
        departamento.agregarCurso(this);
    }

    public String getCodigo() {
        return codigo;
    }

    public String getNombre() {
        return nombre;
    }

    public Departamento getDepartamento() {
        return departamento;
    }
}

// Clase Departamento
class Departamento {
    private String nombre;
    private List<Curso> cursos;

    public Departamento(String nombre) {
        this.nombre = nombre;
        this.cursos = new ArrayList<>();
    }

    public void agregarCurso(Curso curso) {
        cursos.add(curso);
    }

    public List<Curso> consultarCursos() {
        return cursos;
    }

    public String getNombre() {
        return nombre;
    }
}

// Clase Escuela
class Escuela {
    private String nombre;
    private List<Profesor> profesores;

    public Escuela(String nombre) {
        this.nombre = nombre;
        this.profesores = new ArrayList<>();
    }

    public void agregarProfesor(Profesor profesor) {
        profesores.add(profesor);
    }

    public List<Profesor> consultarProfesores() {
        return profesores;
    }

    public String getNombre() {
        return nombre;
    }
}

// Clase principal para ejecutar el sistema
public class Main {
    public static void main(String[] args) {
        // Crear un departamento
        Departamento d1
        
