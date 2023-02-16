import React, { useState } from "react";

const App = () => {
  // Initialiser le niveau et l'expérience
  const [level, setLevel] = useState(1);
  const [experience, setExperience] = useState(0);

  // Fonction pour ajouter de l'expérience
  const handleClick = () => {
    setExperience(experience + 1);
  };

  // Fonction pour ajuster le niveau
  const updateLevel = () => {
    if (experience >= 100) {
      setLevel(level + 1);
      setExperience(0);
    }
  };

  updateLevel();

  return (
    <div>
      <h1>Niveau {level}</h1>
      <div>Expérience {experience}/100</div>
      <progress value={experience} max={100} />
      <button onClick={handleClick}>Effectuer une tâche</button>
    </div>
  );
};
