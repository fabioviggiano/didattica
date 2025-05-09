# Simulazione di campionamento e quantizzazione

accordo = chord(:E3, :minor)

define :suona_originale do
  puts "Suono originale"
  use_synth :piano
  play_pattern_timed accordo, 0.4
  sleep 2
end

define :campionamento_ridotto do
  puts "Simulazione di campionamento a bassa frequenza"
  use_synth :piano
  with_fx :slicer, phase: 0.4, mix: 1 do  # Simula una frequenza di campionamento più bassa
    play_pattern_timed accordo, 0.4, amp: 0.7
  end
  sleep 2
end

define :quantizzazione do
  puts "Simulazione di quantizzazione (riduzione della qualità)"
  use_synth :piano
  with_fx :bitcrusher, bits: 8, sample_rate: 8000 do
    play_pattern_timed accordo, 0.4
  end
  sleep 1
  with_fx :bitcrusher, bits: 4, sample_rate: 4000 do
    play_pattern_timed accordo, 0.4
  end
  sleep 2
end

# Esecuzione in sequenza
suona_originale
campionamento_ridotto
quantizzazione
