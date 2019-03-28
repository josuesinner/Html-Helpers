using System;
using System.Collections.Generic;
using System.Linq;
using System.Web;
using System.ComponentModel.DataAnnotations;

namespace tarea_helpers.Models
{
    public class Datos
    {
        [Required(ErrorMessage ="El Campo Nombre no puede estar vacio")]
        [MinLength(length:1)]
        [MaxLength(length:50)]
        public string nombre { get; set; }
        [Required]
        [MinLength(length: 1)]
        [MaxLength(length: 50)]
        public string apellido { get; set; }
        [Required]
        [Range(15, 99)]
        public int edad { get; set; }
        [Required]
        [MaxLength(length:15)]
        public string telefono { get; set; }
        [Required]
        [MaxLength(length: 14)]
        public string cedula { get; set; }
        [Required]
        [MaxLength(length:50)]
        public string correo { get; set; }
        public string genero { get; set; }
        public string estado_civil { get; set; }
        public string hobbys { get; set; }
    }
}
